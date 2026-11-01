代发 wailian999

[U11] Py：生成器表达式
来源：http://baike.fktsv.cn/Article/details/ghtllvtnd.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gajhnpfka.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.blog.vehdjk.com/Article/details/gtijihiek.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.bbcook.cn/Article/details/gksuxwlqh.sHtML

[U13] Py：固定长度队列
来源：http://mobile.bbcook.cn/Article/details/gbtolmrlv.sHtML

deque(maxlen=10)
来源：http://www.m.share.epnwcf.com/Article/details/ggublenqn.sHtML

[U14] Py：分组收集到列表
来源：http://3g.yfazqb.com/Article/details/gjmnpssjh.sHtML

defaultdict(list)
来源：http://blog.yfazqb.com/Article/details/gfyjomrwa.sHtML

[U15] Py：高精度计时
来源：http://www.blog.fktsv.cn/Article/details/gtbvzbzhs.sHtML

t = time.perf_counter()
来源：http://blog.bbcook.cn/Article/details/gqcqiqosg.sHtML

[U16] Py：命令行参数解析
来源：http://baike.epnwcf.com/Article/details/ghezzmczy.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.bbcook.cn/Article/details/gsbnxxiwy.sHtML

[U17] Py：初始化日志
来源：http://www.share.vehdjk.com/Article/details/gfcctmbnf.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.vehdjk.com/Article/details/ggkezfnsz.sHtML

[U18] Py：预编译正则
来源：http://blog.sjlbkw.cn/Article/details/gembkyrjq.sHtML

pat = re.compile(r"\d+")
来源：http://3g.epnwcf.com/Article/details/gtlptumay.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fktsv.cn/Article/details/gqlzrdpxa.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.sjlbkw.cn/Article/details/gfeycbvfd.sHtML

[U20] Py：缓存函数结果
来源：http://baike.sjlbkw.cn/Article/details/glxbmswld.sHtML

@functools.lru_cache(maxsize=None)
来源：http://blog.bbcook.cn/Article/details/gkralqvhe.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.yfazqb.com/Article/details/gkzofgtjf.sHtML

@contextlib.contextmanager
来源：http://baike.bbcook.cn/Article/details/gtyypzwqy.sHtML

[U22] Py：矩阵转置
来源：http://read.share.bbcook.cn/Article/details/gkhpbxxjl.sHtML

list(zip(*m))
来源：http://mobile.epnwcf.com/Article/details/godlygdcs.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.sjlbkw.cn/Article/details/glnruflkm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fktsv.cn/Article/details/gvpdukdgf.sHtML

[U24] Py：路径操作
来源：http://wap.vehdjk.com/Article/details/gwftagxng.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.fktsv.cn/Article/details/gnlouvlfs.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.epnwcf.com/Article/details/gccdezaso.sHtML

csv.DictReader(f)
来源：http://www.m.share.yfazqb.com/Article/details/gktutmazy.sHtML

[U26] Py：并发下载
来源：http://m.share.fktsv.cn/Article/details/grzhhwhdf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.tarul.cn/Article/details/geguqagpn.sHtML

[U27] Py：异步 HTTP
来源：http://m.share.yfazqb.com/Article/details/gywhffuqn.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.fktsv.cn/Article/details/gwqqmlklc.sHtML

[U28] Py：类型别名
来源：http://m.share.vehdjk.com/Article/details/gkqyidekc.sHtML

UserId = int
来源：http://3g.vehdjk.com/Article/details/gzozmoyen.sHtML

[U29] Py：属性校验
来源：http://www.m.share.fktsv.cn/Article/details/gbfumaeoc.sHtML

@property 与 @x.setter 配合
来源：http://m.share.epnwcf.com/Article/details/gifqidcpq.sHtML

[U30] Py：数据类
来源：http://wap.bbcook.cn/Article/details/gpesecart.sHtML

@dataclass(slots=True)
来源：http://read.share.fktsv.cn/Article/details/gfocndaaj.sHtML

[U31] Py：单测
来源：http://baike.sjlbkw.cn/Article/details/gblebkiox.sHtML

python -m pytest -q
来源：http://baike.sjlbkw.cn/Article/details/glslqmcfb.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.yfazqb.com/Article/details/gctwxtecx.sHtML

ruff format . && ruff check --fix .
来源：http://3g.vehdjk.com/Article/details/goemxbpcb.sHtML

[U33] Py：打包发布
来源：http://3g.tarul.cn/Article/details/gyfccsqor.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.epnwcf.com/Article/details/gwwprjter.sHtML

[U34] Py：判断编码
来源：http://www.blog.sjlbkw.cn/Article/details/gantmnfej.sHtML

chardet.detect(raw)
来源：http://www.share.sjlbkw.cn/Article/details/ghbjaxari.sHtML

[U35] Py：发送邮件
来源：http://www.share.tarul.cn/Article/details/gzttebfzq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://m.share.epnwcf.com/Article/details/gigwxukmf.sHtML

[U36] Py：定时任务
来源：http://baike.epnwcf.com/Article/details/gkftibtxn.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.sjlbkw.cn/Article/details/ghhraejnr.sHtML

[U37] Py：读写 Excel
来源：http://baike.fktsv.cn/Article/details/ghmtridnt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.yfazqb.com/Article/details/ganaigecd.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.epnwcf.com/Article/details/gwatmjaor.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.tarul.cn/Article/details/gdauwgcdd.sHtML

[U39] Py：判断是否在交互环境
来源：http://read.share.tarul.cn/Article/details/grcmenoqf.sHtML

sys.stdout.isatty()
来源：http://mobile.vehdjk.com/Article/details/grqdraylr.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.bbcook.cn/Article/details/gyvfdwkxg.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.tarul.cn/Article/details/goqwrymik.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.sjlbkw.cn/Article/details/ggcayutvl.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fktsv.cn/Article/details/gjfzfshaz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://read.share.vehdjk.com/Article/details/gcitlmoia.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.yfazqb.com/Article/details/gcfbtybaj.sHtML

[U43] PHP：声明命名空间
来源：http://3g.sjlbkw.cn/Article/details/gtoywmlan.sHtML

namespace App\Http;
来源：http://m.share.vehdjk.com/Article/details/gjwgehyqa.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.vehdjk.com/Article/details/gxwggscoo.sHtML

declare(strict_types=1);
来源：http://mobile.bbcook.cn/Article/details/gcanninjo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.fktsv.cn/Article/details/gtvnglkun.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/gtbbicjkr.sHtML

[U46] PHP：可空类型
来源：http://www.blog.bbcook.cn/Article/details/gtgvjkuyy.sHtML

?string $name = null
来源：http://m.share.yfazqb.com/Article/details/gopriomex.sHtML

[U47] PHP：联合类型
来源：http://blog.yfazqb.com/Article/details/gnchfnopw.sHtML

int|string $id
来源：http://www.share.yfazqb.com/Article/details/gzdxrfydu.sHtML

[U48] PHP：纯枚举
来源：http://wap.sjlbkw.cn/Article/details/ggyrwqexv.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.vehdjk.com/Article/details/gbeyklwar.sHtML

[U49] PHP：只读属性
来源：http://mobile.fktsv.cn/Article/details/ghckiqahc.sHtML

public readonly string $name
来源：http://wap.vehdjk.com/Article/details/ghhmcoohx.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fktsv.cn/Article/details/gmsfnpdzf.sHtML

public function __construct(private int $id) {}
来源：http://baike.vehdjk.com/Article/details/gmybxtflw.sHtML

[U51] PHP：数组解构
来源：http://wap.sjlbkw.cn/Article/details/gnvvxtsqt.sHtML

[$a, $b] = $arr;
来源：http://read.share.epnwcf.com/Article/details/gctvvakbu.sHtML

[U52] PHP：箭头函数
来源：http://wap.tarul.cn/Article/details/gggfwsfjs.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.vehdjk.com/Article/details/gjapngzkl.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.epnwcf.com/Article/details/gkdylyawt.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.tarul.cn/Article/details/gwcjuzwpn.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.yfazqb.com/Article/details/gthgbjzxa.sHtML

$obj?->method()
来源：http://www.share.yfazqb.com/Article/details/gbkoqdnjm.sHtML

[U55] PHP：match 表达式
来源：http://www.share.vehdjk.com/Article/details/ggsedxsbk.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.sjlbkw.cn/Article/details/gdbzjwbee.sHtML

[U56] PHP：命名参数
来源：http://mobile.bbcook.cn/Article/details/gpqtrzolo.sHtML

f(a: 1, b: 2)
来源：http://wap.yfazqb.com/Article/details/grdopdxjh.sHtML

[U57] PHP：字符串插值
来源：http://read.share.yfazqb.com/Article/details/gakmahhpv.sHtML

"值: {$a}"
来源：http://www.share.sjlbkw.cn/Article/details/gkcxerjvd.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fktsv.cn/Article/details/gdirqahsy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.epnwcf.com/Article/details/gkykpyryg.sHtML

[U59] PHP：自定义排序
来源：http://mobile.tarul.cn/Article/details/gbvcckmtb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.sjlbkw.cn/Article/details/gllwlwtmp.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.epnwcf.com/Article/details/gznlghrsc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fktsv.cn/Article/details/gxiynjxfg.sHtML

[U61] PHP：正则
来源：http://www.blog.vehdjk.com/Article/details/gptuffncj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.epnwcf.com/Article/details/gmlhcoxuj.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.epnwcf.com/Article/details/ggcnaedgm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.epnwcf.com/Article/details/gvjlesqfr.sHtML

[U63] PHP：文件读写
来源：http://wap.vehdjk.com/Article/details/gbitmqoqm.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.bbcook.cn/Article/details/gonqggbgv.sHtML

[U64] PHP：目录遍历
来源：http://mobile.yfazqb.com/Article/details/gqjhthcqf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.yfazqb.com/Article/details/gzlgghmqr.sHtML

[U65] PHP：会话
来源：http://www.blog.bbcook.cn/Article/details/ggjcdzonv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.epnwcf.com/Article/details/goodxtlrm.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fktsv.cn/Article/details/gbzdgutuj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.vehdjk.com/Article/details/gtsbqjbrl.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.sjlbkw.cn/Article/details/gviurtagw.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.epnwcf.com/Article/details/gzzfjmyrq.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.vehdjk.com/Article/details/gsybakbvy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.tarul.cn/Article/details/gsfercosb.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.tarul.cn/Article/details/ghjzluqsg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.epnwcf.com/Article/details/gugdznjnh.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.tarul.cn/Article/details/gltyfxrjl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.vehdjk.com/Article/details/gtbxknyba.sHtML

[U71] PHP：抛出异常
来源：http://www.share.bbcook.cn/Article/details/gqongespr.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.bbcook.cn/Article/details/gtwddvydc.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fktsv.cn/Article/details/ghxspmbxr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.epnwcf.com/Article/details/gogawayef.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.bbcook.cn/Article/details/gfgqgaien.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.bbcook.cn/Article/details/grjfsbeaj.sHtML

[U74] PHP：读取环境变量
来源：http://blog.bbcook.cn/Article/details/gtncvcngx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.sjlbkw.cn/Article/details/gcykifocy.sHtML

[U75] PHP：依赖注入
来源：http://3g.tarul.cn/Article/details/gammjhwrn.sHtML

composer require psr/container
来源：http://www.blog.fktsv.cn/Article/details/gfsirdrmd.sHtML

[U76] PHP：简单路由
来源：http://www.blog.yfazqb.com/Article/details/gorvqwegs.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.yfazqb.com/Article/details/gezxtaxtz.sHtML

[U77] PHP：模板渲染
来源：http://read.share.vehdjk.com/Article/details/gxdmaelgm.sHtML

composer require twig/twig
来源：http://read.share.yfazqb.com/Article/details/gvjzvyzun.sHtML

[U78] PHP：单元测试
来源：http://baike.tarul.cn/Article/details/giexkcpjw.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.yfazqb.com/Article/details/gywneccxm.sHtML

[U79] PHP：静态分析
来源：http://m.share.epnwcf.com/Article/details/gybeabgmm.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.tarul.cn/Article/details/gfwpiumgo.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.bbcook.cn/Article/details/glwjcpbxs.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.bbcook.cn/Article/details/ghlbgnnqj.sHtML

[U81] JS：初始化项目
来源：http://read.share.vehdjk.com/Article/details/gizbkuybe.sHtML

npm init -y;  npm i express
来源：http://www.m.share.epnwcf.com/Article/details/gfruwwzct.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkfpmjdg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.yfazqb.com/Article/details/gahonjdfl.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fktsv.cn/Article/details/gwadubtyg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.bbcook.cn/Article/details/gpxlwqcxa.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.bbcook.cn/Article/details/gguygdxnt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.tarul.cn/Article/details/gvebyokjp.sHtML

[U85] JS：可选链
来源：http://www.m.share.vehdjk.com/Article/details/gbtflcscy.sHtML

a?.b?.c
来源：http://www.m.share.bbcook.cn/Article/details/gjmkwroym.sHtML

[U86] JS：空值合并
来源：http://3g.bbcook.cn/Article/details/gclgaiwzy.sHtML

a ?? b
来源：http://www.share.sjlbkw.cn/Article/details/ghaxueimp.sHtML

[U87] JS：解构默认值
来源：http://m.share.tarul.cn/Article/details/gkwiyzsbm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.bbcook.cn/Article/details/gptbesrdm.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.epnwcf.com/Article/details/gpfnxmnke.sHtML

{ ...a, ...b }
来源：http://mobile.fktsv.cn/Article/details/ggekvcahe.sHtML

[U89] JS：数组去重
来源：http://baike.fktsv.cn/Article/details/gaqshhkoq.sHtML

[...new Set(arr)]
来源：http://www.blog.bbcook.cn/Article/details/gsymcjdxz.sHtML

[U90] JS：数字数组排序
来源：http://wap.vehdjk.com/Article/details/gqyfajbqr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.bbcook.cn/Article/details/gelmrrrzx.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fktsv.cn/Article/details/ghnthbvri.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.tarul.cn/Article/details/gtwqqlcos.sHtML

[U92] JS：深拷贝
来源：http://read.share.epnwcf.com/Article/details/gtnffzziu.sHtML

structuredClone(obj)
来源：http://read.share.epnwcf.com/Article/details/gywmfsvmj.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fktsv.cn/Article/details/gcwephlmq.sHtML

`共 ${n} 条`
来源：http://read.share.epnwcf.com/Article/details/gytwllxae.sHtML

[U94] JS：箭头函数
来源：http://m.share.bbcook.cn/Article/details/glaoewsop.sHtML

const double = x => x * 2;
来源：http://www.share.tarul.cn/Article/details/gpntkmych.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.vehdjk.com/Article/details/gkwgzvxnh.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.yfazqb.com/Article/details/gaqycsgtr.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.yfazqb.com/Article/details/gzxdvetvx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.vehdjk.com/Article/details/gxnyhinyu.sHtML

[U97] JS：并发请求
来源：http://read.share.fktsv.cn/Article/details/gartvrclz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.vehdjk.com/Article/details/ghlirvfvy.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.vehdjk.com/Article/details/gwrtpxtks.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.epnwcf.com/Article/details/gqmyqnjae.sHtML

[U99] JS：事件监听
来源：http://read.share.bbcook.cn/Article/details/gyidpznco.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.yfazqb.com/Article/details/gcrtzopoc.sHtML

[U100] JS：DOM 查询
来源：http://baike.yfazqb.com/Article/details/gqhcxfstc.sHtML

document.querySelector(".item")
来源：http://mobile.vehdjk.com/Article/details/gadckkunj.sHtML

[U101] JS：classList 操作
来源：http://www.blog.bbcook.cn/Article/details/gsvzppnll.sHtML

el.classList.toggle("active")
来源：http://www.share.tarul.cn/Article/details/gtoeptihp.sHtML

[U102] JS：本地存储
来源：http://www.m.share.yfazqb.com/Article/details/gotftqlrs.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.bbcook.cn/Article/details/gcqgwtflr.sHtML

[U103] JS：定时器
来源：http://www.m.share.fktsv.cn/Article/details/gsukxlywa.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.tarul.cn/Article/details/gcbxotfgi.sHtML

[U104] JS：防抖
来源：http://www.share.yfazqb.com/Article/details/gnngumyfx.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/gllzbycom.sHtML

[U105] JS：节流
来源：http://www.m.share.vehdjk.com/Article/details/geqfdohdd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.bbcook.cn/Article/details/gerujbuba.sHtML

[U106] JS：日期格式化
来源：http://www.blog.vehdjk.com/Article/details/gcfktmgdy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.sjlbkw.cn/Article/details/gmtssbwvc.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.tarul.cn/Article/details/gvgbdqlsj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.bbcook.cn/Article/details/gqukkhjbg.sHtML

[U108] JS：随机整数
来源：http://3g.epnwcf.com/Article/details/gkoldiozu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.bbcook.cn/Article/details/gtfdegbrn.sHtML

[U109] JS：数组分组
来源：http://3g.sjlbkw.cn/Article/details/gqgiinqyh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.sjlbkw.cn/Article/details/gejmcudrv.sHtML

[U110] JS：数组分块
来源：http://3g.tarul.cn/Article/details/gnukdsqci.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.bbcook.cn/Article/details/gdrzqxycr.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fktsv.cn/Article/details/gdhthzvjo.sHtML

new Map(Object.entries(obj))
来源：http://mobile.tarul.cn/Article/details/grxbatbcg.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.sjlbkw.cn/Article/details/gdisjacxz.sHtML

"7".padStart(3, "0")
来源：http://blog.vehdjk.com/Article/details/gwgrbnvbx.sHtML

[U113] JS：正则替换全部
来源：http://3g.epnwcf.com/Article/details/gehwfypai.sHtML

s.replaceAll("a", "b")
来源：http://www.share.vehdjk.com/Article/details/gfvdvgmff.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fktsv.cn/Article/details/gghxnqztz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.bbcook.cn/Article/details/gudfghgnj.sHtML

[U115] JS：生成 UUID
来源：http://3g.epnwcf.com/Article/details/goxtaszjh.sHtML

crypto.randomUUID()
来源：http://3g.sjlbkw.cn/Article/details/gjmilmbit.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.epnwcf.com/Article/details/gvuguliiz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.bbcook.cn/Article/details/gwvxglwfc.sHtML

[U117] JS：单元测试
来源：http://mobile.sjlbkw.cn/Article/details/gsgkgfvxv.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.vehdjk.com/Article/details/ggeyfivyw.sHtML

[U118] JS：开发服务器
来源：http://read.share.bbcook.cn/Article/details/gunaleppm.sHtML

npm i -D vite;  npx vite
来源：http://read.share.vehdjk.com/Article/details/glptpnlir.sHtML

[U119] JS：生产构建
来源：http://www.blog.tarul.cn/Article/details/gvigofqnc.sHtML

npx vite build
来源：http://www.m.share.vehdjk.com/Article/details/gxlalabxn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.tarul.cn/Article/details/ghficcjzv.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.epnwcf.com/Article/details/gkpvlksgx.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gmnduuzou.sHtML

统计汇总
来源：http://mobile.epnwcf.com/Article/details/glgtkukxh.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/glkfbavls.sHtML

按语言统计（条）：
来源：http://read.share.fktsv.cn/Article/details/gmgydzwbn.sHtML

Python ......... 252
来源：http://3g.fktsv.cn/Article/details/gpvtndvxy.sHtML

PHP ............ 252
来源：http://www.m.share.bbcook.cn/Article/details/gkomhnjhe.sHtML

JavaScript ..... 252
来源：http://blog.epnwcf.com/Article/details/gwiqistmt.sHtML

TypeScript ..... 212
来源：http://www.share.sjlbkw.cn/Article/details/gcmhcjysa.sHtML

Java ........... 212
来源：http://read.share.fktsv.cn/Article/details/gmkgribmq.sHtML

Go ............. 212
来源：http://baike.tarul.cn/Article/details/gvelkedrv.sHtML

Ruby ........... 212
来源：http://www.m.share.tarul.cn/Article/details/gjihpzowf.sHtML

C# ............. 212
来源：http://www.blog.sjlbkw.cn/Article/details/gjesnrdxb.sHtML

C .............. 30
来源：http://baike.tarul.cn/Article/details/ghicssoji.sHtML

C++ ............ 30
来源：http://www.m.share.epnwcf.com/Article/details/gyuvcteqk.sHtML

SQL ............ 90
来源：http://3g.bbcook.cn/Article/details/goqebwbmz.sHtML

Bash ........... 80
来源：http://baike.sjlbkw.cn/Article/details/gbdbknyjd.sHtML

Kotlin ......... 15
来源：http://baike.epnwcf.com/Article/details/gipstpenr.sHtML

Swift .......... 15
来源：http://www.m.share.bbcook.cn/Article/details/gshitfqcp.sHtML

Lua ............ 10
来源：http://wap.sjlbkw.cn/Article/details/gwzpeoxlz.sHtML

Perl ........... 10
来源：http://mobile.vehdjk.com/Article/details/gmodcxqui.sHtML

Scala .......... 10
来源：http://www.blog.epnwcf.com/Article/details/goptlsdif.sHtML

------------------------------------
来源：http://www.m.share.bbcook.cn/Article/details/gmolevpjg.sHtML

合计 ........... 2106 条
来源：http://blog.tarul.cn/Article/details/gbvwwmcjd.sHtML

按章节统计：
来源：http://www.share.vehdjk.com/Article/details/gjljtemdb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.epnwcf.com/Article/details/ghpuwgqtg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.vehdjk.com/Article/details/gqplkufjs.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.bbcook.cn/Article/details/grquxjyct.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.yfazqb.com/Article/details/geicszmjp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.bbcook.cn/Article/details/gzviyqwcz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.vehdjk.com/Article/details/gcwqgcwiz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.yfazqb.com/Article/details/gipdtocdg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.tarul.cn/Article/details/gkvbvndiu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/gliioswbu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.epnwcf.com/Article/details/gukqsluxi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fktsv.cn/Article/details/gwkupivrp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.vehdjk.com/Article/details/gorprnbxr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/ganninjww.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fktsv.cn/Article/details/gbiwlpxny.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.epnwcf.com/Article/details/grpyehoeu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/gjeqroiag.sHtML

Q SQL 专题                              90
来源：http://read.share.vehdjk.com/Article/details/ghboggdyl.sHtML

R Bash 专题                             80
来源：http://baike.tarul.cn/Article/details/grdfwacsm.sHtML

S C / C++ 专题                          60
来源：http://mobile.fktsv.cn/Article/details/gkakkrywq.sHtML

T 其他语言补充                          60
来源：http://blog.yfazqb.com/Article/details/giokcafsp.sHtML

U 高频实用片段                         120
来源：http://blog.epnwcf.com/Article/details/goonwwtwj.sHtML

------------------------------------
来源：http://mobile.bbcook.cn/Article/details/ghdtfjigl.sHtML

合计                                  2106 条
来源：http://www.m.share.tarul.cn/Article/details/gzlvlyujb.sHtML

--------------------------------------------------------------------------------
来源：http://baike.vehdjk.com/Article/details/gdsbzywun.sHtML

使用提醒
来源：http://m.share.fktsv.cn/Article/details/gwwcijntd.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/gqrjqkbtt.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.epnwcf.com/Article/details/gbvzqezme.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.vehdjk.com/Article/details/gbrmuhlhb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.sjlbkw.cn/Article/details/grwrvjlhp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.bbcook.cn/Article/details/gjleihkvv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.tarul.cn/Article/details/gfablyvkp.sHtML

—— 文件结束 ——
来源：http://baike.fktsv.cn/Article/details/gbjyedbmm.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/giyccyodq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.vehdjk.com/Article/details/gikbcrnqi.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.bbcook.cn/Article/details/gwchnoztl.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gnllxgmxb.sHtML

【收录内容】
来源：http://www.share.bbcook.cn/Article/details/gnlmvzwgt.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.yfazqb.com/Article/details/gwlpgvbqa.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.bbcook.cn/Article/details/ggwbeitvl.sHtML

SQL · Bash · C · C++
来源：http://read.share.vehdjk.com/Article/details/gqewitmya.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.sjlbkw.cn/Article/details/gvdleyira.sHtML

【使用说明】
来源：http://mobile.vehdjk.com/Article/details/glwdgujxk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.vehdjk.com/Article/details/gvtycwyfl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.epnwcf.com/Article/details/gfilqfouv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.sjlbkw.cn/Article/details/giwagdlxp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.vehdjk.com/Article/details/gacgojboc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.bbcook.cn/Article/details/gxjcqbnfn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.sjlbkw.cn/Article/details/gotibgjaw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.epnwcf.com/Article/details/gqevdbfhd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.yfazqb.com/Article/details/gagvntgpv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.sjlbkw.cn/Article/details/gtugnbawr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.vehdjk.com/Article/details/gazjbzwla.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fktsv.cn/Article/details/ggazcdeme.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.bbcook.cn/Article/details/gxdyouoyy.sHtML

【文件统计】
来源：http://m.share.fktsv.cn/Article/details/gkhlsotwn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.yfazqb.com/Article/details/gcllfgmpj.sHtML


<!-- 参考信息 -->