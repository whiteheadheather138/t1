代发 wailian999

[U07] Py：反转字典键值
来源：http://blog.yfazqb.com/Article/details/gqzfzvzke.sHtML

{v: k for k, v in d.items()}
来源：http://blog.epnwcf.com/Article/details/gdmhgqlfw.sHtML

[U08] Py：展平二维列表
来源：http://www.share.fktsv.cn/Article/details/gzfmrtbnz.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.tarul.cn/Article/details/gwluaiffg.sHtML

[U09] Py：字典取最大值的键
来源：http://read.share.fktsv.cn/Article/details/gvrdzyinl.sHtML

max(d, key=d.get)
来源：http://www.blog.fktsv.cn/Article/details/gvsjncmtx.sHtML

[U10] Py：按值排序字典
来源：http://3g.epnwcf.com/Article/details/gjozgqrsr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.epnwcf.com/Article/details/gzmqqagzh.sHtML

[U11] Py：生成器表达式
来源：http://www.share.sjlbkw.cn/Article/details/gcgxixkba.sHtML

(x * 2 for x in arr)
来源：http://baike.sjlbkw.cn/Article/details/gdhlguoqw.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.sjlbkw.cn/Article/details/glstbuszd.sHtML

Counter(arr).most_common(3)
来源：http://3g.sjlbkw.cn/Article/details/gnwtarahd.sHtML

[U13] Py：固定长度队列
来源：http://blog.fktsv.cn/Article/details/gntvwxzkb.sHtML

deque(maxlen=10)
来源：http://3g.fktsv.cn/Article/details/grytlznsh.sHtML

[U14] Py：分组收集到列表
来源：http://baike.tarul.cn/Article/details/gcusfqxsa.sHtML

defaultdict(list)
来源：http://m.share.bbcook.cn/Article/details/gjzivnlju.sHtML

[U15] Py：高精度计时
来源：http://3g.tarul.cn/Article/details/gsxjmxkxx.sHtML

t = time.perf_counter()
来源：http://blog.sjlbkw.cn/Article/details/gzkvqeahs.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.tarul.cn/Article/details/gvhzrxsax.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.fktsv.cn/Article/details/gakqpukuh.sHtML

[U17] Py：初始化日志
来源：http://mobile.epnwcf.com/Article/details/gutlwagta.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.bbcook.cn/Article/details/gprsggovd.sHtML

[U18] Py：预编译正则
来源：http://mobile.bbcook.cn/Article/details/gimxznoqt.sHtML

pat = re.compile(r"\d+")
来源：http://m.share.vehdjk.com/Article/details/gppgyuhsb.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.yfazqb.com/Article/details/gtmngyoaj.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://baike.vehdjk.com/Article/details/givjppexn.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.sjlbkw.cn/Article/details/gdionhvni.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.yfazqb.com/Article/details/gnoepvirl.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.sjlbkw.cn/Article/details/gcyxddzek.sHtML

@contextlib.contextmanager
来源：http://www.share.sjlbkw.cn/Article/details/gezpplnsm.sHtML

[U22] Py：矩阵转置
来源：http://m.share.yfazqb.com/Article/details/gtdljsqxd.sHtML

list(zip(*m))
来源：http://3g.epnwcf.com/Article/details/ghhfgqasd.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.sjlbkw.cn/Article/details/ggtiyjcya.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.epnwcf.com/Article/details/gwctvafij.sHtML

[U24] Py：路径操作
来源：http://www.share.tarul.cn/Article/details/gswsemxpz.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.bbcook.cn/Article/details/gbodoztye.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.vehdjk.com/Article/details/gdvzeqhxf.sHtML

csv.DictReader(f)
来源：http://www.share.yfazqb.com/Article/details/gnljxqubf.sHtML

[U26] Py：并发下载
来源：http://www.m.share.tarul.cn/Article/details/goycbsxuj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.sjlbkw.cn/Article/details/gkrcnijan.sHtML

[U27] Py：异步 HTTP
来源：http://3g.epnwcf.com/Article/details/glonjgdyu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.fktsv.cn/Article/details/ghwjvfgsm.sHtML

[U28] Py：类型别名
来源：http://wap.fktsv.cn/Article/details/gcplqsply.sHtML

UserId = int
来源：http://read.share.sjlbkw.cn/Article/details/gkbsuavuw.sHtML

[U29] Py：属性校验
来源：http://blog.tarul.cn/Article/details/gvxibljrl.sHtML

@property 与 @x.setter 配合
来源：http://3g.epnwcf.com/Article/details/gcwdplict.sHtML

[U30] Py：数据类
来源：http://baike.tarul.cn/Article/details/gdtsvimps.sHtML

@dataclass(slots=True)
来源：http://m.share.epnwcf.com/Article/details/gonveppkd.sHtML

[U31] Py：单测
来源：http://3g.yfazqb.com/Article/details/grarcxllu.sHtML

python -m pytest -q
来源：http://read.share.yfazqb.com/Article/details/ghchbfibl.sHtML

[U32] Py：代码格式化
来源：http://read.share.vehdjk.com/Article/details/gpkhkdjhj.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.yfazqb.com/Article/details/gbppxjzdn.sHtML

[U33] Py：打包发布
来源：http://m.share.fktsv.cn/Article/details/gmqgkodtg.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.vehdjk.com/Article/details/givydnyfq.sHtML

[U34] Py：判断编码
来源：http://www.m.share.vehdjk.com/Article/details/giabgjiwx.sHtML

chardet.detect(raw)
来源：http://read.share.tarul.cn/Article/details/gpptcnugb.sHtML

[U35] Py：发送邮件
来源：http://baike.bbcook.cn/Article/details/guhddqrqf.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.vehdjk.com/Article/details/gtbapvpbb.sHtML

[U36] Py：定时任务
来源：http://baike.bbcook.cn/Article/details/glarqcque.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.sjlbkw.cn/Article/details/ggmlqxnnk.sHtML

[U37] Py：读写 Excel
来源：http://wap.tarul.cn/Article/details/ghzqvscvs.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.epnwcf.com/Article/details/gpomgjvjp.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.yfazqb.com/Article/details/ggnrcdhvn.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.epnwcf.com/Article/details/gtysntuey.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.fktsv.cn/Article/details/gacllvnvy.sHtML

sys.stdout.isatty()
来源：http://baike.bbcook.cn/Article/details/gbgzpbilu.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.tarul.cn/Article/details/gkivmtwxh.sHtML

print("err", file=sys.stderr)
来源：http://wap.bbcook.cn/Article/details/gbuodbmvg.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.fktsv.cn/Article/details/gqltzfxxm.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fktsv.cn/Article/details/gcyuwskug.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.vehdjk.com/Article/details/gfeiadpbg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.sjlbkw.cn/Article/details/gwcfgokwx.sHtML

[U43] PHP：声明命名空间
来源：http://blog.bbcook.cn/Article/details/ghgjjmwvv.sHtML

namespace App\Http;
来源：http://wap.sjlbkw.cn/Article/details/gwdyqtyto.sHtML

[U44] PHP：开启严格类型
来源：http://baike.fktsv.cn/Article/details/gxwnyjigy.sHtML

declare(strict_types=1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjyptbuot.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.epnwcf.com/Article/details/goaieizzw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.epnwcf.com/Article/details/gzkvipapa.sHtML

[U46] PHP：可空类型
来源：http://blog.tarul.cn/Article/details/gbudetqev.sHtML

?string $name = null
来源：http://wap.tarul.cn/Article/details/ghhdavihk.sHtML

[U47] PHP：联合类型
来源：http://www.share.fktsv.cn/Article/details/gpfrprfcj.sHtML

int|string $id
来源：http://read.share.vehdjk.com/Article/details/gnumaubeg.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fktsv.cn/Article/details/gbfqrzprt.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://blog.epnwcf.com/Article/details/gvkwjgalt.sHtML

[U49] PHP：只读属性
来源：http://www.share.fktsv.cn/Article/details/gkqqbnffy.sHtML

public readonly string $name
来源：http://3g.bbcook.cn/Article/details/gefbmimju.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.fktsv.cn/Article/details/grtyputua.sHtML

public function __construct(private int $id) {}
来源：http://m.share.yfazqb.com/Article/details/gszibjkcu.sHtML

[U51] PHP：数组解构
来源：http://blog.bbcook.cn/Article/details/gemimpsgy.sHtML

[$a, $b] = $arr;
来源：http://mobile.bbcook.cn/Article/details/gpdmqvzqp.sHtML

[U52] PHP：箭头函数
来源：http://mobile.bbcook.cn/Article/details/gyemxxjrh.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.epnwcf.com/Article/details/gaemdmqik.sHtML

[U53] PHP：空合并运算符
来源：http://3g.sjlbkw.cn/Article/details/gsurgzbpb.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.yfazqb.com/Article/details/gayktagrz.sHtML

[U54] PHP：空安全调用
来源：http://wap.sjlbkw.cn/Article/details/gznupihjs.sHtML

$obj?->method()
来源：http://blog.epnwcf.com/Article/details/gcnrxyftn.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.epnwcf.com/Article/details/ggmyawyuv.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fktsv.cn/Article/details/gowhcxtar.sHtML

[U56] PHP：命名参数
来源：http://baike.yfazqb.com/Article/details/gtckvegqk.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fktsv.cn/Article/details/gvyabufvw.sHtML

[U57] PHP：字符串插值
来源：http://blog.yfazqb.com/Article/details/gucqjbedn.sHtML

"值: {$a}"
来源：http://mobile.epnwcf.com/Article/details/gvnyjbnfu.sHtML

[U58] PHP：数组三件套
来源：http://m.share.bbcook.cn/Article/details/goenxeuqt.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.tarul.cn/Article/details/gqdoaihoq.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.bbcook.cn/Article/details/gmefmmzed.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fktsv.cn/Article/details/gpkjwktui.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fktsv.cn/Article/details/ganfnqurh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.sjlbkw.cn/Article/details/ghrtheogx.sHtML

[U61] PHP：正则
来源：http://read.share.vehdjk.com/Article/details/gsnhrjfsb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfnvvgdwf.sHtML

[U62] PHP：日期对象
来源：http://3g.sjlbkw.cn/Article/details/gtkwamblq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.sjlbkw.cn/Article/details/gnbycsjxo.sHtML

[U63] PHP：文件读写
来源：http://mobile.bbcook.cn/Article/details/gzweypvuz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.yfazqb.com/Article/details/goaaqccle.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fktsv.cn/Article/details/gvkxgyylv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.bbcook.cn/Article/details/gwfrvcxqq.sHtML

[U65] PHP：会话
来源：http://www.m.share.fktsv.cn/Article/details/gejtospkr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.vehdjk.com/Article/details/gjnruwtsi.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.sjlbkw.cn/Article/details/gsbcxaneo.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.sjlbkw.cn/Article/details/gezkhnklz.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.yfazqb.com/Article/details/gohzywdfi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fktsv.cn/Article/details/gaozrlrhx.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.bbcook.cn/Article/details/gtvkwzaff.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.vehdjk.com/Article/details/gjrdbolxm.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.yfazqb.com/Article/details/gmpbhkqig.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.vehdjk.com/Article/details/grocdiycz.sHtML

[U70] PHP：PDO 事务
来源：http://3g.sjlbkw.cn/Article/details/gzvonhcep.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.bbcook.cn/Article/details/gjofgdvls.sHtML

[U71] PHP：抛出异常
来源：http://m.share.vehdjk.com/Article/details/gbislocfz.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.yfazqb.com/Article/details/gpdhjbudi.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fktsv.cn/Article/details/grvcnuied.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.tarul.cn/Article/details/gmxrogsrn.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.bbcook.cn/Article/details/grcwpbveh.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.sjlbkw.cn/Article/details/gddzawvuf.sHtML

[U74] PHP：读取环境变量
来源：http://3g.sjlbkw.cn/Article/details/gyjttprmo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.bbcook.cn/Article/details/gnjniazse.sHtML

[U75] PHP：依赖注入
来源：http://baike.sjlbkw.cn/Article/details/gcigwccjf.sHtML

composer require psr/container
来源：http://blog.bbcook.cn/Article/details/galsiwqei.sHtML

[U76] PHP：简单路由
来源：http://3g.fktsv.cn/Article/details/gjhlojtku.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.epnwcf.com/Article/details/gxwbsmjmb.sHtML

[U77] PHP：模板渲染
来源：http://wap.epnwcf.com/Article/details/gbfdczmsw.sHtML

composer require twig/twig
来源：http://mobile.sjlbkw.cn/Article/details/gekrhluan.sHtML

[U78] PHP：单元测试
来源：http://mobile.vehdjk.com/Article/details/gelyjmjgr.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.yfazqb.com/Article/details/gqmikqbwb.sHtML

[U79] PHP：静态分析
来源：http://baike.tarul.cn/Article/details/gmsqbzugy.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.sjlbkw.cn/Article/details/grbpzxnxf.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.sjlbkw.cn/Article/details/glcbosmee.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.fktsv.cn/Article/details/geduyyvbz.sHtML

[U81] JS：初始化项目
来源：http://mobile.yfazqb.com/Article/details/gjyjncmzt.sHtML

npm init -y;  npm i express
来源：http://read.share.sjlbkw.cn/Article/details/ghgxgytfk.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.vehdjk.com/Article/details/gqusnechb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.epnwcf.com/Article/details/ggfoajajj.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.epnwcf.com/Article/details/gdputfcqa.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.vehdjk.com/Article/details/gssvrkybc.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fktsv.cn/Article/details/ggyadopto.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.tarul.cn/Article/details/grngmhbrv.sHtML

[U85] JS：可选链
来源：http://baike.bbcook.cn/Article/details/gnxgqbrmr.sHtML

a?.b?.c
来源：http://mobile.fktsv.cn/Article/details/gqnykxrnv.sHtML

[U86] JS：空值合并
来源：http://baike.fktsv.cn/Article/details/gzjiyqtnv.sHtML

a ?? b
来源：http://baike.bbcook.cn/Article/details/gwrdiauok.sHtML

[U87] JS：解构默认值
来源：http://m.share.epnwcf.com/Article/details/gjubiyqjk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fktsv.cn/Article/details/gxocfibvo.sHtML

[U88] JS：对象展开合并
来源：http://blog.bbcook.cn/Article/details/gmnpeccwx.sHtML

{ ...a, ...b }
来源：http://read.share.fktsv.cn/Article/details/gwgztbzzd.sHtML

[U89] JS：数组去重
来源：http://wap.bbcook.cn/Article/details/guwspvrvv.sHtML

[...new Set(arr)]
来源：http://www.blog.yfazqb.com/Article/details/gjkepfjrf.sHtML

[U90] JS：数字数组排序
来源：http://mobile.epnwcf.com/Article/details/gonontvpc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/grnpidmar.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.sjlbkw.cn/Article/details/gjhdlxiwx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.tarul.cn/Article/details/gfiyfhoco.sHtML

[U92] JS：深拷贝
来源：http://baike.vehdjk.com/Article/details/gcyrdpmbv.sHtML

structuredClone(obj)
来源：http://blog.bbcook.cn/Article/details/gyzunnjhk.sHtML

[U93] JS：模板字符串
来源：http://www.blog.epnwcf.com/Article/details/gvnslqons.sHtML

`共 ${n} 条`
来源：http://m.share.yfazqb.com/Article/details/grrozjqts.sHtML

[U94] JS：箭头函数
来源：http://3g.yfazqb.com/Article/details/gvibaxngl.sHtML

const double = x => x * 2;
来源：http://3g.tarul.cn/Article/details/gbyldnpmx.sHtML

[U95] JS：Promise 包装
来源：http://mobile.yfazqb.com/Article/details/gqpvcudjd.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.sjlbkw.cn/Article/details/godcgcuya.sHtML

[U96] JS：async/await 与异常
来源：http://3g.vehdjk.com/Article/details/gshsjmkxu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.vehdjk.com/Article/details/gphyjgucd.sHtML

[U97] JS：并发请求
来源：http://www.share.bbcook.cn/Article/details/gvhtsbosv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/gljhiiydt.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fktsv.cn/Article/details/gnrsnlznd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.tarul.cn/Article/details/gzfbhotnh.sHtML

[U99] JS：事件监听
来源：http://mobile.fktsv.cn/Article/details/gzokcomij.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fktsv.cn/Article/details/gajlicfxm.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.vehdjk.com/Article/details/gtjevrjje.sHtML

document.querySelector(".item")
来源：http://www.m.share.bbcook.cn/Article/details/gtvezkkvq.sHtML

[U101] JS：classList 操作
来源：http://3g.fktsv.cn/Article/details/glfnocehx.sHtML

el.classList.toggle("active")
来源：http://m.share.fktsv.cn/Article/details/gemhanvev.sHtML

[U102] JS：本地存储
来源：http://www.blog.bbcook.cn/Article/details/gfvojniuf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.epnwcf.com/Article/details/ghtvbzjdp.sHtML

[U103] JS：定时器
来源：http://m.share.yfazqb.com/Article/details/gurdcmaiy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.epnwcf.com/Article/details/gpokeiuow.sHtML

[U104] JS：防抖
来源：http://wap.epnwcf.com/Article/details/ghqafypwk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.bbcook.cn/Article/details/gefbjkanc.sHtML

[U105] JS：节流
来源：http://m.share.yfazqb.com/Article/details/gktcsveoo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fktsv.cn/Article/details/ggeitnigl.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmvxqztr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.epnwcf.com/Article/details/gqxdlwabf.sHtML

[U107] JS：数字千分位
来源：http://baike.yfazqb.com/Article/details/ghhfafefk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.sjlbkw.cn/Article/details/gdnkfszyq.sHtML

[U108] JS：随机整数
来源：http://blog.fktsv.cn/Article/details/gmjmdojxq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fktsv.cn/Article/details/gnhupsxxs.sHtML

[U109] JS：数组分组
来源：http://3g.sjlbkw.cn/Article/details/glowbdseh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fktsv.cn/Article/details/gygqdcuaj.sHtML

[U110] JS：数组分块
来源：http://blog.epnwcf.com/Article/details/gslunowdc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.tarul.cn/Article/details/gajhyaomy.sHtML

[U111] JS：对象转 Map
来源：http://mobile.yfazqb.com/Article/details/gjxeoxvdu.sHtML

new Map(Object.entries(obj))
来源：http://m.share.bbcook.cn/Article/details/gevpudtob.sHtML

[U112] JS：字符串补位
来源：http://www.share.fktsv.cn/Article/details/gzkcawphh.sHtML

"7".padStart(3, "0")
来源：http://3g.epnwcf.com/Article/details/gnaucazvn.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.vehdjk.com/Article/details/gdpfdftgm.sHtML

s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gjvliduqo.sHtML

[U114] JS：JSON 深比较
来源：http://wap.epnwcf.com/Article/details/ghndethcr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fktsv.cn/Article/details/gypnuxcfg.sHtML

[U115] JS：生成 UUID
来源：http://wap.bbcook.cn/Article/details/gqkhbtyyo.sHtML

crypto.randomUUID()
来源：http://www.m.share.bbcook.cn/Article/details/gqeyflrrr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.tarul.cn/Article/details/ggcxedfjg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.bbcook.cn/Article/details/gxyllbdec.sHtML

[U117] JS：单元测试
来源：http://baike.yfazqb.com/Article/details/gmvibhvcy.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.epnwcf.com/Article/details/glrjpurvk.sHtML

[U118] JS：开发服务器
来源：http://m.share.yfazqb.com/Article/details/gohkrwahl.sHtML

npm i -D vite;  npx vite
来源：http://baike.tarul.cn/Article/details/gndobxxcm.sHtML

[U119] JS：生产构建
来源：http://mobile.epnwcf.com/Article/details/gwrjosvkd.sHtML

npx vite build
来源：http://www.share.bbcook.cn/Article/details/gqtjxticd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.epnwcf.com/Article/details/grfrwgatd.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.epnwcf.com/Article/details/gyoralgua.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gqqpdyluw.sHtML

统计汇总
来源：http://read.share.tarul.cn/Article/details/glvxqjvcv.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gpncsaypz.sHtML

按语言统计（条）：
来源：http://wap.sjlbkw.cn/Article/details/ggslobxsy.sHtML

Python ......... 252
来源：http://3g.vehdjk.com/Article/details/ghljgevgn.sHtML

PHP ............ 252
来源：http://baike.vehdjk.com/Article/details/ggnnuxbne.sHtML

JavaScript ..... 252
来源：http://www.share.epnwcf.com/Article/details/ghtzzydca.sHtML

TypeScript ..... 212
来源：http://mobile.vehdjk.com/Article/details/gyfpsasaa.sHtML

Java ........... 212
来源：http://3g.sjlbkw.cn/Article/details/gjatlejxf.sHtML

Go ............. 212
来源：http://3g.tarul.cn/Article/details/gaoixlbpu.sHtML

Ruby ........... 212
来源：http://read.share.tarul.cn/Article/details/glyslaaud.sHtML

C# ............. 212
来源：http://www.m.share.fktsv.cn/Article/details/gmiibvogv.sHtML

C .............. 30
来源：http://3g.tarul.cn/Article/details/ggcaysgug.sHtML

C++ ............ 30
来源：http://m.share.fktsv.cn/Article/details/gbprzuojp.sHtML

SQL ............ 90
来源：http://blog.yfazqb.com/Article/details/gxxeloiyy.sHtML

Bash ........... 80
来源：http://baike.vehdjk.com/Article/details/goqqgpuvu.sHtML

Kotlin ......... 15
来源：http://www.m.share.sjlbkw.cn/Article/details/gjkhavlks.sHtML

Swift .......... 15
来源：http://www.m.share.bbcook.cn/Article/details/gmiexlqjk.sHtML

Lua ............ 10
来源：http://wap.sjlbkw.cn/Article/details/gsobwirms.sHtML

Perl ........... 10
来源：http://baike.fktsv.cn/Article/details/gwxvhhufu.sHtML

Scala .......... 10
来源：http://www.m.share.bbcook.cn/Article/details/gwrqvlruo.sHtML

------------------------------------
来源：http://blog.tarul.cn/Article/details/ghxtbktbe.sHtML

合计 ........... 2106 条
来源：http://www.share.vehdjk.com/Article/details/gkpdofnsl.sHtML

按章节统计：
来源：http://www.share.fktsv.cn/Article/details/gnrdsmtqz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.bbcook.cn/Article/details/gavwwhnqv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fktsv.cn/Article/details/gnduiugdw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.vehdjk.com/Article/details/ghxqkumhy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.tarul.cn/Article/details/gmzqzeoie.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.sjlbkw.cn/Article/details/gsmirizbm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.epnwcf.com/Article/details/gblshbagk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.bbcook.cn/Article/details/gbxbyerlv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fktsv.cn/Article/details/gtunndmrj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fktsv.cn/Article/details/gmjsvqhjt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fktsv.cn/Article/details/gaekiegtg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/gdwmmsnih.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fktsv.cn/Article/details/gokihdupu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/gveybacuc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.sjlbkw.cn/Article/details/grnacvqln.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.sjlbkw.cn/Article/details/gcnivrvxi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.yfazqb.com/Article/details/gechfuaof.sHtML

Q SQL 专题                              90
来源：http://m.share.yfazqb.com/Article/details/gijylbzhg.sHtML

R Bash 专题                             80
来源：http://www.m.share.yfazqb.com/Article/details/gifxkregc.sHtML

S C / C++ 专题                          60
来源：http://www.blog.yfazqb.com/Article/details/gjwxajhhk.sHtML

T 其他语言补充                          60
来源：http://wap.epnwcf.com/Article/details/gutkvqvkm.sHtML

U 高频实用片段                         120
来源：http://3g.bbcook.cn/Article/details/guirdmuac.sHtML

------------------------------------
来源：http://wap.vehdjk.com/Article/details/gyhnikypx.sHtML

合计                                  2106 条
来源：http://read.share.sjlbkw.cn/Article/details/gbprzwfgn.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.tarul.cn/Article/details/gycqvrjoe.sHtML

使用提醒
来源：http://mobile.vehdjk.com/Article/details/gqifhvcvc.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.bbcook.cn/Article/details/gnkgevtnp.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.epnwcf.com/Article/details/gkchszbqo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.sjlbkw.cn/Article/details/gedzdqukb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.yfazqb.com/Article/details/grvpuzhsq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.vehdjk.com/Article/details/grakhvpkh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.epnwcf.com/Article/details/gdpdqxtpo.sHtML

—— 文件结束 ——
来源：http://mobile.bbcook.cn/Article/details/gfrpbeehy.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gfaunuqdh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.tarul.cn/Article/details/gsoavpaqn.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fktsv.cn/Article/details/giojaqrqm.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/ghspbwlaf.sHtML

【收录内容】
来源：http://blog.epnwcf.com/Article/details/gckoicwdc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.bbcook.cn/Article/details/gffiqkfqx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.epnwcf.com/Article/details/gptiheyty.sHtML

SQL · Bash · C · C++
来源：http://www.share.yfazqb.com/Article/details/gffepprhm.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fktsv.cn/Article/details/gbwgpyzab.sHtML

【使用说明】
来源：http://www.blog.yfazqb.com/Article/details/gkcxnpxnh.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.tarul.cn/Article/details/gqcaxgkme.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.bbcook.cn/Article/details/ghcbpclop.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.yfazqb.com/Article/details/gtmowrjvr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.yfazqb.com/Article/details/ggawxntyt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.epnwcf.com/Article/details/ghnpdyjmf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.yfazqb.com/Article/details/gfysuzzzz.sHtML


<!-- 参考信息 -->