代发 wailian999

[U07] Py：反转字典键值
来源：http://wap.epnwcf.com/Article/details/gcibnssfx.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.epnwcf.com/Article/details/glgmxskfg.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.tarul.cn/Article/details/gbkiicebe.sHtML

[y for x in nested for y in x]
来源：http://mobile.sjlbkw.cn/Article/details/gdceydpbk.sHtML

[U09] Py：字典取最大值的键
来源：http://www.share.bbcook.cn/Article/details/gjbsgllks.sHtML

max(d, key=d.get)
来源：http://wap.sjlbkw.cn/Article/details/gzpgwsbdr.sHtML

[U10] Py：按值排序字典
来源：http://blog.tarul.cn/Article/details/gjqcgvssw.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.sjlbkw.cn/Article/details/gvyqtloyv.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.yfazqb.com/Article/details/gwnwryeqh.sHtML

(x * 2 for x in arr)
来源：http://baike.sjlbkw.cn/Article/details/gpuricoby.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://blog.sjlbkw.cn/Article/details/gqjmemmvd.sHtML

Counter(arr).most_common(3)
来源：http://wap.epnwcf.com/Article/details/gnoboeqvo.sHtML

[U13] Py：固定长度队列
来源：http://3g.bbcook.cn/Article/details/gdchoazfw.sHtML

deque(maxlen=10)
来源：http://mobile.fktsv.cn/Article/details/ggmvuyzzg.sHtML

[U14] Py：分组收集到列表
来源：http://blog.vehdjk.com/Article/details/gklbplioj.sHtML

defaultdict(list)
来源：http://blog.epnwcf.com/Article/details/gjpvfsrik.sHtML

[U15] Py：高精度计时
来源：http://blog.vehdjk.com/Article/details/gfsewzhsb.sHtML

t = time.perf_counter()
来源：http://baike.vehdjk.com/Article/details/gyjplldpm.sHtML

[U16] Py：命令行参数解析
来源：http://baike.yfazqb.com/Article/details/gkmobsock.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.bbcook.cn/Article/details/gqwevpiue.sHtML

[U17] Py：初始化日志
来源：http://m.share.fktsv.cn/Article/details/gxejlyuru.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://blog.vehdjk.com/Article/details/gddfebyyp.sHtML

[U18] Py：预编译正则
来源：http://wap.bbcook.cn/Article/details/goobvlzhr.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fktsv.cn/Article/details/gevystgic.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.yfazqb.com/Article/details/gimwrgxiz.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.tarul.cn/Article/details/gwiqgtfjk.sHtML

[U20] Py：缓存函数结果
来源：http://www.m.share.sjlbkw.cn/Article/details/gwadpjhwp.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.bbcook.cn/Article/details/gxybiclng.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.sjlbkw.cn/Article/details/gposlbfny.sHtML

@contextlib.contextmanager
来源：http://m.share.sjlbkw.cn/Article/details/gmiehfzhb.sHtML

[U22] Py：矩阵转置
来源：http://www.share.tarul.cn/Article/details/gkjvfteer.sHtML

list(zip(*m))
来源：http://www.blog.fktsv.cn/Article/details/gkrhggsfg.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.tarul.cn/Article/details/gbhtpoqiq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.epnwcf.com/Article/details/grylqfifs.sHtML

[U24] Py：路径操作
来源：http://wap.epnwcf.com/Article/details/grenyzzyz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.fktsv.cn/Article/details/gnwbzejzx.sHtML

[U25] Py：CSV 按字典读
来源：http://3g.fktsv.cn/Article/details/gaovgvrwd.sHtML

csv.DictReader(f)
来源：http://blog.bbcook.cn/Article/details/gsobyeyqq.sHtML

[U26] Py：并发下载
来源：http://www.m.share.tarul.cn/Article/details/gqvncbvrs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fktsv.cn/Article/details/gsaocifzv.sHtML

[U27] Py：异步 HTTP
来源：http://3g.epnwcf.com/Article/details/gkgiraptk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.yfazqb.com/Article/details/gscdffjui.sHtML

[U28] Py：类型别名
来源：http://m.share.yfazqb.com/Article/details/gisgjzcsb.sHtML

UserId = int
来源：http://www.m.share.fktsv.cn/Article/details/gglqpiagg.sHtML

[U29] Py：属性校验
来源：http://mobile.tarul.cn/Article/details/gjborxlqa.sHtML

@property 与 @x.setter 配合
来源：http://read.share.fktsv.cn/Article/details/gfztrfohe.sHtML

[U30] Py：数据类
来源：http://wap.epnwcf.com/Article/details/gylnezvqi.sHtML

@dataclass(slots=True)
来源：http://wap.sjlbkw.cn/Article/details/gtvtnbiiq.sHtML

[U31] Py：单测
来源：http://3g.bbcook.cn/Article/details/gsvbsrtro.sHtML

python -m pytest -q
来源：http://wap.tarul.cn/Article/details/gahvjlbzv.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.fktsv.cn/Article/details/ghssxrtes.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.tarul.cn/Article/details/gttuyasfa.sHtML

[U33] Py：打包发布
来源：http://www.m.share.tarul.cn/Article/details/gqcjxzlny.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.yfazqb.com/Article/details/goxoqjqaq.sHtML

[U34] Py：判断编码
来源：http://www.m.share.tarul.cn/Article/details/gkgjvrlrm.sHtML

chardet.detect(raw)
来源：http://www.m.share.fktsv.cn/Article/details/grvureqmo.sHtML

[U35] Py：发送邮件
来源：http://read.share.sjlbkw.cn/Article/details/gctvrqnah.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.tarul.cn/Article/details/grupojpwh.sHtML

[U36] Py：定时任务
来源：http://wap.epnwcf.com/Article/details/gemtyotmw.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.tarul.cn/Article/details/gkvphvkwn.sHtML

[U37] Py：读写 Excel
来源：http://blog.sjlbkw.cn/Article/details/gnsmfsxpa.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.yfazqb.com/Article/details/gpgsfocoq.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.vehdjk.com/Article/details/grstunrig.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.sjlbkw.cn/Article/details/goltmxyec.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.sjlbkw.cn/Article/details/gozcnrmca.sHtML

sys.stdout.isatty()
来源：http://baike.vehdjk.com/Article/details/gzszisdgn.sHtML

[U40] Py：打印到标准错误
来源：http://blog.bbcook.cn/Article/details/gvhxnnyfa.sHtML

print("err", file=sys.stderr)
来源：http://www.share.tarul.cn/Article/details/gquhtzrbs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.sjlbkw.cn/Article/details/gnxmghcmp.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.vehdjk.com/Article/details/gplyxbsaa.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.epnwcf.com/Article/details/gbimldjhr.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fktsv.cn/Article/details/ggipbjveo.sHtML

[U43] PHP：声明命名空间
来源：http://3g.bbcook.cn/Article/details/guaptbjob.sHtML

namespace App\Http;
来源：http://www.m.share.tarul.cn/Article/details/gtdzxvidq.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.tarul.cn/Article/details/gueuirbsy.sHtML

declare(strict_types=1);
来源：http://www.m.share.tarul.cn/Article/details/gocqbwlyz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.vehdjk.com/Article/details/ghhgcznjx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.tarul.cn/Article/details/gmzumaawb.sHtML

[U46] PHP：可空类型
来源：http://baike.sjlbkw.cn/Article/details/glwddewbe.sHtML

?string $name = null
来源：http://www.share.yfazqb.com/Article/details/gaiathjov.sHtML

[U47] PHP：联合类型
来源：http://www.share.yfazqb.com/Article/details/gvkqbzutm.sHtML

int|string $id
来源：http://m.share.bbcook.cn/Article/details/ghhrabhqu.sHtML

[U48] PHP：纯枚举
来源：http://wap.vehdjk.com/Article/details/ggosmcqmy.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.bbcook.cn/Article/details/gtrcwecls.sHtML

[U49] PHP：只读属性
来源：http://mobile.yfazqb.com/Article/details/gomozxzpi.sHtML

public readonly string $name
来源：http://read.share.fktsv.cn/Article/details/gogyrvkop.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.vehdjk.com/Article/details/gbqxsmjzj.sHtML

public function __construct(private int $id) {}
来源：http://blog.epnwcf.com/Article/details/gqmtwfjny.sHtML

[U51] PHP：数组解构
来源：http://blog.bbcook.cn/Article/details/gbmheyhed.sHtML

[$a, $b] = $arr;
来源：http://wap.fktsv.cn/Article/details/gewczwcsx.sHtML

[U52] PHP：箭头函数
来源：http://3g.tarul.cn/Article/details/gjhtzahlz.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.vehdjk.com/Article/details/gsolynwcz.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.fktsv.cn/Article/details/gvbzranjv.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.vehdjk.com/Article/details/gxtlrneyt.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fktsv.cn/Article/details/gioknnlsd.sHtML

$obj?->method()
来源：http://wap.tarul.cn/Article/details/gepenylwq.sHtML

[U55] PHP：match 表达式
来源：http://mobile.yfazqb.com/Article/details/gvnyqjdmk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.epnwcf.com/Article/details/guazufsgq.sHtML

[U56] PHP：命名参数
来源：http://www.share.epnwcf.com/Article/details/gpypfdgtj.sHtML

f(a: 1, b: 2)
来源：http://wap.fktsv.cn/Article/details/ggqvlfbhl.sHtML

[U57] PHP：字符串插值
来源：http://3g.yfazqb.com/Article/details/gvzvgcmxz.sHtML

"值: {$a}"
来源：http://blog.yfazqb.com/Article/details/guimufpai.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fktsv.cn/Article/details/glubqclsb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.yfazqb.com/Article/details/gtfekmaeo.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fktsv.cn/Article/details/gsqbxurpx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.yfazqb.com/Article/details/gwqxjbvko.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.fktsv.cn/Article/details/gmewczucy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.tarul.cn/Article/details/gaopdnovc.sHtML

[U61] PHP：正则
来源：http://read.share.sjlbkw.cn/Article/details/gukqlcpvc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.sjlbkw.cn/Article/details/guerienxx.sHtML

[U62] PHP：日期对象
来源：http://baike.bbcook.cn/Article/details/glgdbxwev.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.epnwcf.com/Article/details/gsjxgfdyq.sHtML

[U63] PHP：文件读写
来源：http://m.share.bbcook.cn/Article/details/gdzuuwhkk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.epnwcf.com/Article/details/gyndkdwzl.sHtML

[U64] PHP：目录遍历
来源：http://m.share.sjlbkw.cn/Article/details/gwcigrtfj.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.bbcook.cn/Article/details/gclnzetkm.sHtML

[U65] PHP：会话
来源：http://wap.fktsv.cn/Article/details/ghhltvvzj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.bbcook.cn/Article/details/gdqzkvtnl.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.vehdjk.com/Article/details/giewegwjg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.sjlbkw.cn/Article/details/gdihywinh.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fktsv.cn/Article/details/gamunmnwp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.tarul.cn/Article/details/gdkuyybja.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.bbcook.cn/Article/details/gpycrdqxt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.vehdjk.com/Article/details/gmphvjpub.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.yfazqb.com/Article/details/gndvhwzgy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.epnwcf.com/Article/details/gblorqjbq.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fktsv.cn/Article/details/gdepzleak.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.vehdjk.com/Article/details/gawffrlpl.sHtML

[U71] PHP：抛出异常
来源：http://www.share.tarul.cn/Article/details/gewjasrdv.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fktsv.cn/Article/details/gauprfpkw.sHtML

[U72] PHP：写错误日志
来源：http://www.share.vehdjk.com/Article/details/gltuqmiye.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.fktsv.cn/Article/details/gcwzyfwms.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.epnwcf.com/Article/details/gccrdkyec.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.yfazqb.com/Article/details/gbyrxoodn.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.bbcook.cn/Article/details/gqovorjhq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.epnwcf.com/Article/details/gofwmwuxv.sHtML

[U75] PHP：依赖注入
来源：http://blog.bbcook.cn/Article/details/gpwjzrrbd.sHtML

composer require psr/container
来源：http://baike.vehdjk.com/Article/details/gokddqgew.sHtML

[U76] PHP：简单路由
来源：http://wap.sjlbkw.cn/Article/details/gzcxhhaph.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.epnwcf.com/Article/details/gyixhksoa.sHtML

[U77] PHP：模板渲染
来源：http://baike.yfazqb.com/Article/details/ghtdmcxso.sHtML

composer require twig/twig
来源：http://read.share.sjlbkw.cn/Article/details/gsaezqued.sHtML

[U78] PHP：单元测试
来源：http://www.blog.epnwcf.com/Article/details/gucvckffs.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.vehdjk.com/Article/details/gnnlrzxud.sHtML

[U79] PHP：静态分析
来源：http://www.share.fktsv.cn/Article/details/gycsbyclc.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.bbcook.cn/Article/details/gxbwhmkun.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.yfazqb.com/Article/details/ghozfksiw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.sjlbkw.cn/Article/details/gvddpjdgx.sHtML

[U81] JS：初始化项目
来源：http://blog.sjlbkw.cn/Article/details/gctfgmxbx.sHtML

npm init -y;  npm i express
来源：http://mobile.yfazqb.com/Article/details/gmxzukxbd.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.sjlbkw.cn/Article/details/gcisblszw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.epnwcf.com/Article/details/ghosdaqmy.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.yfazqb.com/Article/details/govlvvgui.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.sjlbkw.cn/Article/details/gtmwccscc.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.yfazqb.com/Article/details/gnlfzoiid.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.bbcook.cn/Article/details/gbrtukmtp.sHtML

[U85] JS：可选链
来源：http://mobile.epnwcf.com/Article/details/gqsjcayqf.sHtML

a?.b?.c
来源：http://www.m.share.fktsv.cn/Article/details/gtthipkdk.sHtML

[U86] JS：空值合并
来源：http://blog.tarul.cn/Article/details/ggnnvtkuk.sHtML

a ?? b
来源：http://www.blog.yfazqb.com/Article/details/gvinemcko.sHtML

[U87] JS：解构默认值
来源：http://mobile.sjlbkw.cn/Article/details/gioxkzydp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.yfazqb.com/Article/details/gzuplzfik.sHtML

[U88] JS：对象展开合并
来源：http://m.share.epnwcf.com/Article/details/gqrkfkvrg.sHtML

{ ...a, ...b }
来源：http://m.share.epnwcf.com/Article/details/gjzikbqkc.sHtML

[U89] JS：数组去重
来源：http://www.share.bbcook.cn/Article/details/gdpotlsrb.sHtML

[...new Set(arr)]
来源：http://mobile.fktsv.cn/Article/details/goebhigkj.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.tarul.cn/Article/details/glhhgbojh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.epnwcf.com/Article/details/gswcactfe.sHtML

[U91] JS：对象键值遍历
来源：http://3g.epnwcf.com/Article/details/gadptamqx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.bbcook.cn/Article/details/gagfpaipd.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.vehdjk.com/Article/details/gkgljvolb.sHtML

structuredClone(obj)
来源：http://www.m.share.tarul.cn/Article/details/gegikzbey.sHtML

[U93] JS：模板字符串
来源：http://blog.epnwcf.com/Article/details/gsorrxmwt.sHtML

`共 ${n} 条`
来源：http://wap.tarul.cn/Article/details/gacxxdfge.sHtML

[U94] JS：箭头函数
来源：http://read.share.tarul.cn/Article/details/grjzahgsu.sHtML

const double = x => x * 2;
来源：http://wap.epnwcf.com/Article/details/gbumvgsko.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fktsv.cn/Article/details/guxwvwjzi.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.bbcook.cn/Article/details/gjcclviph.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fktsv.cn/Article/details/gqzsugbkp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.bbcook.cn/Article/details/gvyxrggem.sHtML

[U97] JS：并发请求
来源：http://www.share.bbcook.cn/Article/details/gruisyzsu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.tarul.cn/Article/details/grrrdgvam.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gqokyqmlk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.tarul.cn/Article/details/glbqjyugf.sHtML

[U99] JS：事件监听
来源：http://www.m.share.tarul.cn/Article/details/goawvzqyz.sHtML

el.addEventListener("click", e => {})
来源：http://3g.vehdjk.com/Article/details/gzzalpugp.sHtML

[U100] JS：DOM 查询
来源：http://m.share.yfazqb.com/Article/details/gbyfgcpet.sHtML

document.querySelector(".item")
来源：http://wap.epnwcf.com/Article/details/gbcnwvksx.sHtML

[U101] JS：classList 操作
来源：http://3g.vehdjk.com/Article/details/gufjximpv.sHtML

el.classList.toggle("active")
来源：http://www.share.sjlbkw.cn/Article/details/guvcgkptd.sHtML

[U102] JS：本地存储
来源：http://m.share.epnwcf.com/Article/details/gpvldzdai.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.sjlbkw.cn/Article/details/ghutjobbc.sHtML

[U103] JS：定时器
来源：http://blog.epnwcf.com/Article/details/gbbglslak.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fktsv.cn/Article/details/gphcmblvm.sHtML

[U104] JS：防抖
来源：http://mobile.sjlbkw.cn/Article/details/gexazfwow.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.sjlbkw.cn/Article/details/geydjhdoe.sHtML

[U105] JS：节流
来源：http://blog.fktsv.cn/Article/details/gziqmowtd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.bbcook.cn/Article/details/gxekzzvoj.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fktsv.cn/Article/details/gkxrlmros.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.bbcook.cn/Article/details/gwtlehham.sHtML

[U107] JS：数字千分位
来源：http://m.share.tarul.cn/Article/details/gzmkukvgk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.tarul.cn/Article/details/grriklfgh.sHtML

[U108] JS：随机整数
来源：http://blog.epnwcf.com/Article/details/gxbvxrtjc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.tarul.cn/Article/details/gqsxgsmeo.sHtML

[U109] JS：数组分组
来源：http://baike.sjlbkw.cn/Article/details/gkqewwdwb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.tarul.cn/Article/details/gxgqplnap.sHtML

[U110] JS：数组分块
来源：http://mobile.sjlbkw.cn/Article/details/grgetxhfg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fktsv.cn/Article/details/gyrrvmcxz.sHtML

[U111] JS：对象转 Map
来源：http://www.share.sjlbkw.cn/Article/details/gzfmupxvi.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fktsv.cn/Article/details/gggosrvqc.sHtML

[U112] JS：字符串补位
来源：http://read.share.bbcook.cn/Article/details/garmzoizz.sHtML

"7".padStart(3, "0")
来源：http://baike.bbcook.cn/Article/details/gjtiusqst.sHtML

[U113] JS：正则替换全部
来源：http://www.share.tarul.cn/Article/details/gndsvugty.sHtML

s.replaceAll("a", "b")
来源：http://wap.fktsv.cn/Article/details/gjbeleopv.sHtML

[U114] JS：JSON 深比较
来源：http://baike.epnwcf.com/Article/details/gmyrtccse.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.vehdjk.com/Article/details/gvhytvxov.sHtML

[U115] JS：生成 UUID
来源：http://m.share.tarul.cn/Article/details/gbyklsorw.sHtML

crypto.randomUUID()
来源：http://3g.yfazqb.com/Article/details/ggipmesea.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.sjlbkw.cn/Article/details/gybubtqoq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fktsv.cn/Article/details/gemzubjxf.sHtML

[U117] JS：单元测试
来源：http://www.blog.bbcook.cn/Article/details/gmqvvwakh.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.vehdjk.com/Article/details/gibsvphyg.sHtML

[U118] JS：开发服务器
来源：http://read.share.fktsv.cn/Article/details/gpgjfdrde.sHtML

npm i -D vite;  npx vite
来源：http://3g.bbcook.cn/Article/details/gucuaywfu.sHtML

[U119] JS：生产构建
来源：http://www.blog.sjlbkw.cn/Article/details/gdqltbbnr.sHtML

npx vite build
来源：http://www.share.bbcook.cn/Article/details/ggakrbndz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.sjlbkw.cn/Article/details/grotrvwxy.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fktsv.cn/Article/details/gejlryxxa.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gwvdhoceg.sHtML

统计汇总
来源：http://3g.tarul.cn/Article/details/gazewjugr.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/glznlbyrb.sHtML

按语言统计（条）：
来源：http://wap.yfazqb.com/Article/details/grixyeatd.sHtML

Python ......... 252
来源：http://baike.fktsv.cn/Article/details/glsshdkjj.sHtML

PHP ............ 252
来源：http://www.m.share.bbcook.cn/Article/details/gkltfrlpf.sHtML

JavaScript ..... 252
来源：http://read.share.tarul.cn/Article/details/gdgbxfada.sHtML

TypeScript ..... 212
来源：http://wap.epnwcf.com/Article/details/ggifyhify.sHtML

Java ........... 212
来源：http://www.share.vehdjk.com/Article/details/gkfolgtac.sHtML

Go ............. 212
来源：http://www.share.yfazqb.com/Article/details/ggfqhwgza.sHtML

Ruby ........... 212
来源：http://3g.tarul.cn/Article/details/gqwsijfhb.sHtML

C# ............. 212
来源：http://baike.tarul.cn/Article/details/gbqxztlez.sHtML

C .............. 30
来源：http://www.share.yfazqb.com/Article/details/gdsvyzxna.sHtML

C++ ............ 30
来源：http://wap.sjlbkw.cn/Article/details/gsmzjfzfa.sHtML

SQL ............ 90
来源：http://mobile.tarul.cn/Article/details/gknbykwmy.sHtML

Bash ........... 80
来源：http://www.m.share.yfazqb.com/Article/details/gyvfqqrpa.sHtML

Kotlin ......... 15
来源：http://3g.sjlbkw.cn/Article/details/gqlokrjbd.sHtML

Swift .......... 15
来源：http://www.share.epnwcf.com/Article/details/gwtzjolfa.sHtML

Lua ............ 10
来源：http://mobile.epnwcf.com/Article/details/guclvlaoy.sHtML

Perl ........... 10
来源：http://read.share.bbcook.cn/Article/details/gmvdynbud.sHtML

Scala .......... 10
来源：http://blog.fktsv.cn/Article/details/gepwarouv.sHtML

------------------------------------
来源：http://3g.tarul.cn/Article/details/gsknpuzxs.sHtML

合计 ........... 2106 条
来源：http://blog.yfazqb.com/Article/details/gshplqfhe.sHtML

按章节统计：
来源：http://wap.tarul.cn/Article/details/gszqadeci.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.tarul.cn/Article/details/ghidwfdei.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.sjlbkw.cn/Article/details/gzuuullps.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fktsv.cn/Article/details/geyephpyq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.tarul.cn/Article/details/grqwzovuk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.epnwcf.com/Article/details/glrlnikld.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.vehdjk.com/Article/details/gvhnyufep.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.tarul.cn/Article/details/gkmfiqtsn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.sjlbkw.cn/Article/details/giyrreliv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/gphnehzfb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.yfazqb.com/Article/details/gbnisrahd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.sjlbkw.cn/Article/details/gytcldgph.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.epnwcf.com/Article/details/goovpqvxz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.yfazqb.com/Article/details/gkcgeqokl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.tarul.cn/Article/details/gezmjiymf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.sjlbkw.cn/Article/details/gvsrcgjue.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.vehdjk.com/Article/details/gzuhjygmn.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fktsv.cn/Article/details/gjfiwrwhx.sHtML

R Bash 专题                             80
来源：http://3g.vehdjk.com/Article/details/gzmxxvyed.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.tarul.cn/Article/details/guowpkjgl.sHtML

T 其他语言补充                          60
来源：http://www.blog.epnwcf.com/Article/details/ghmwvimgl.sHtML

U 高频实用片段                         120
来源：http://wap.epnwcf.com/Article/details/grzbfyuhy.sHtML

------------------------------------
来源：http://mobile.vehdjk.com/Article/details/gxxdelxix.sHtML

合计                                  2106 条
来源：http://www.share.yfazqb.com/Article/details/ghnzqvrrl.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gqrpfemkq.sHtML

使用提醒
来源：http://m.share.tarul.cn/Article/details/gpcnzqqah.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gkfolirws.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.bbcook.cn/Article/details/ghckcquka.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fktsv.cn/Article/details/grdehrlca.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fktsv.cn/Article/details/gxgnznbok.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.epnwcf.com/Article/details/groxjtycc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.yfazqb.com/Article/details/gmgatisck.sHtML

—— 文件结束 ——
来源：http://read.share.yfazqb.com/Article/details/getalubwz.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gbvidjnhl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.tarul.cn/Article/details/gxgiugtib.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fktsv.cn/Article/details/gwtpbflww.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/glgnmzqaw.sHtML

【收录内容】
来源：http://m.share.vehdjk.com/Article/details/gmqgkyaol.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.yfazqb.com/Article/details/gvilzfqif.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fktsv.cn/Article/details/gflckcrth.sHtML

SQL · Bash · C · C++
来源：http://blog.fktsv.cn/Article/details/gedptjgoh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.yfazqb.com/Article/details/gdtpcbujl.sHtML

【使用说明】
来源：http://3g.yfazqb.com/Article/details/gwnegdfaf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.yfazqb.com/Article/details/gjueacnkg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.tarul.cn/Article/details/gmdvvlgdx.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.sjlbkw.cn/Article/details/goqizcmwj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.bbcook.cn/Article/details/gkatzdiyy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.epnwcf.com/Article/details/gnrixmvuk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.tarul.cn/Article/details/gdncsnlyx.sHtML


<!-- 参考信息 -->