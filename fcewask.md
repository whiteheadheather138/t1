代发 wailian999

[U05] Py：列表去重且保序
来源：http://read.share.sjlbkw.cn/Article/details/gaeuhdweb.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.tarul.cn/Article/details/gfeafeaey.sHtML

[U06] Py：合并两个字典
来源：http://www.share.epnwcf.com/Article/details/ggotnhjsz.sHtML

{**a, **b}
来源：http://www.blog.bbcook.cn/Article/details/gtimjzuje.sHtML

[U07] Py：反转字典键值
来源：http://3g.bbcook.cn/Article/details/gdniuqckv.sHtML

{v: k for k, v in d.items()}
来源：http://blog.fktsv.cn/Article/details/gpodcmvlp.sHtML

[U08] Py：展平二维列表
来源：http://wap.fktsv.cn/Article/details/gibovmjgs.sHtML

[y for x in nested for y in x]
来源：http://wap.vehdjk.com/Article/details/gershhlwk.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fktsv.cn/Article/details/gfsspdzbp.sHtML

max(d, key=d.get)
来源：http://wap.yfazqb.com/Article/details/gylwkbczi.sHtML

[U10] Py：按值排序字典
来源：http://www.share.vehdjk.com/Article/details/gexnoarxd.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.sjlbkw.cn/Article/details/gceujfvlk.sHtML

[U11] Py：生成器表达式
来源：http://baike.vehdjk.com/Article/details/gvkhawsgi.sHtML

(x * 2 for x in arr)
来源：http://3g.sjlbkw.cn/Article/details/ggpdwtmvl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.bbcook.cn/Article/details/gilpkduue.sHtML

Counter(arr).most_common(3)
来源：http://www.share.epnwcf.com/Article/details/gaorkiixk.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fktsv.cn/Article/details/gcltbenww.sHtML

deque(maxlen=10)
来源：http://3g.bbcook.cn/Article/details/gvgibuown.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.tarul.cn/Article/details/gxqmbfzyq.sHtML

defaultdict(list)
来源：http://wap.tarul.cn/Article/details/gxgpotdgq.sHtML

[U15] Py：高精度计时
来源：http://www.share.yfazqb.com/Article/details/gbaslovpm.sHtML

t = time.perf_counter()
来源：http://baike.yfazqb.com/Article/details/grzhxxjnu.sHtML

[U16] Py：命令行参数解析
来源：http://baike.tarul.cn/Article/details/goqtjiblm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.yfazqb.com/Article/details/ghqrdaxya.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.fktsv.cn/Article/details/gsvlqioio.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.epnwcf.com/Article/details/ghtegtujb.sHtML

[U18] Py：预编译正则
来源：http://blog.bbcook.cn/Article/details/guxtbfcgr.sHtML

pat = re.compile(r"\d+")
来源：http://blog.bbcook.cn/Article/details/gbxlmpdis.sHtML

[U19] Py：正则替换带回调
来源：http://read.share.yfazqb.com/Article/details/gveqpfdce.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://3g.sjlbkw.cn/Article/details/gnphayith.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.bbcook.cn/Article/details/gqpbwrkhq.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.tarul.cn/Article/details/ghqtipaiv.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fktsv.cn/Article/details/gpnrbklom.sHtML

@contextlib.contextmanager
来源：http://wap.vehdjk.com/Article/details/gqhgsgwdh.sHtML

[U22] Py：矩阵转置
来源：http://blog.tarul.cn/Article/details/ggydylodp.sHtML

list(zip(*m))
来源：http://3g.tarul.cn/Article/details/glvtzyqig.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.tarul.cn/Article/details/gtswtkqvx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://m.share.vehdjk.com/Article/details/gpdnipaij.sHtML

[U24] Py：路径操作
来源：http://read.share.yfazqb.com/Article/details/gxqbocvma.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.fktsv.cn/Article/details/gcvfprnaf.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.epnwcf.com/Article/details/gvbtmqisx.sHtML

csv.DictReader(f)
来源：http://read.share.vehdjk.com/Article/details/ghobfndho.sHtML

[U26] Py：并发下载
来源：http://www.m.share.epnwcf.com/Article/details/golxyqhkg.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.yfazqb.com/Article/details/gykafxtpd.sHtML

[U27] Py：异步 HTTP
来源：http://wap.fktsv.cn/Article/details/gxdckklfl.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.epnwcf.com/Article/details/gubvnhpho.sHtML

[U28] Py：类型别名
来源：http://mobile.vehdjk.com/Article/details/gyfxgadqz.sHtML

UserId = int
来源：http://www.blog.yfazqb.com/Article/details/gwrlamgrx.sHtML

[U29] Py：属性校验
来源：http://www.blog.tarul.cn/Article/details/gmlhtoylw.sHtML

@property 与 @x.setter 配合
来源：http://m.share.tarul.cn/Article/details/gciikugpn.sHtML

[U30] Py：数据类
来源：http://read.share.yfazqb.com/Article/details/gfrbnjuty.sHtML

@dataclass(slots=True)
来源：http://m.share.sjlbkw.cn/Article/details/gsameghio.sHtML

[U31] Py：单测
来源：http://read.share.bbcook.cn/Article/details/gqfikddny.sHtML

python -m pytest -q
来源：http://baike.tarul.cn/Article/details/gsylemmuo.sHtML

[U32] Py：代码格式化
来源：http://read.share.epnwcf.com/Article/details/gedmriznb.sHtML

ruff format . && ruff check --fix .
来源：http://read.share.bbcook.cn/Article/details/gvnkbwgjp.sHtML

[U33] Py：打包发布
来源：http://www.blog.fktsv.cn/Article/details/gpnylukow.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.bbcook.cn/Article/details/gdfffpsiy.sHtML

[U34] Py：判断编码
来源：http://www.blog.yfazqb.com/Article/details/gaqaujbzr.sHtML

chardet.detect(raw)
来源：http://mobile.bbcook.cn/Article/details/gdgxbhxqc.sHtML

[U35] Py：发送邮件
来源：http://wap.epnwcf.com/Article/details/gttqkmist.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.epnwcf.com/Article/details/gusufsgxo.sHtML

[U36] Py：定时任务
来源：http://read.share.vehdjk.com/Article/details/gznundufc.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.sjlbkw.cn/Article/details/gjtnxqzmb.sHtML

[U37] Py：读写 Excel
来源：http://read.share.epnwcf.com/Article/details/gyczadjjl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.tarul.cn/Article/details/gjgptxhvz.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.vehdjk.com/Article/details/gmqaheifc.sHtML

Path(__file__).resolve().parent
来源：http://mobile.bbcook.cn/Article/details/gtdbizozv.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.yfazqb.com/Article/details/gdilqzonf.sHtML

sys.stdout.isatty()
来源：http://www.blog.epnwcf.com/Article/details/gebpcwrgf.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fktsv.cn/Article/details/ghnxfgubt.sHtML

print("err", file=sys.stderr)
来源：http://blog.tarul.cn/Article/details/glvgsyjui.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.yfazqb.com/Article/details/gpcvhulri.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.sjlbkw.cn/Article/details/glbrcmump.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.bbcook.cn/Article/details/gvjyrqhzv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.yfazqb.com/Article/details/gkgpbjbew.sHtML

[U43] PHP：声明命名空间
来源：http://wap.tarul.cn/Article/details/gvrezdiis.sHtML

namespace App\Http;
来源：http://wap.fktsv.cn/Article/details/gzqrdavmj.sHtML

[U44] PHP：开启严格类型
来源：http://3g.tarul.cn/Article/details/glfflrttp.sHtML

declare(strict_types=1);
来源：http://blog.vehdjk.com/Article/details/gsuoltval.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.sjlbkw.cn/Article/details/ghfntkhvb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/gdwuvisqk.sHtML

[U46] PHP：可空类型
来源：http://www.share.fktsv.cn/Article/details/gjswtczjt.sHtML

?string $name = null
来源：http://m.share.epnwcf.com/Article/details/gcgygoevg.sHtML

[U47] PHP：联合类型
来源：http://mobile.epnwcf.com/Article/details/ghgtpjngn.sHtML

int|string $id
来源：http://www.blog.fktsv.cn/Article/details/gvhstspyv.sHtML

[U48] PHP：纯枚举
来源：http://www.share.tarul.cn/Article/details/gskgofhfp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.epnwcf.com/Article/details/gkgbukree.sHtML

[U49] PHP：只读属性
来源：http://m.share.tarul.cn/Article/details/gzqsriaxw.sHtML

public readonly string $name
来源：http://www.m.share.tarul.cn/Article/details/gnkyclqjn.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.sjlbkw.cn/Article/details/gwvvycdxt.sHtML

public function __construct(private int $id) {}
来源：http://read.share.epnwcf.com/Article/details/glliwzzwa.sHtML

[U51] PHP：数组解构
来源：http://read.share.yfazqb.com/Article/details/gmlwncocc.sHtML

[$a, $b] = $arr;
来源：http://blog.vehdjk.com/Article/details/gximgadqs.sHtML

[U52] PHP：箭头函数
来源：http://baike.tarul.cn/Article/details/gjvltexee.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkspfrnv.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.tarul.cn/Article/details/ghaeyukze.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.epnwcf.com/Article/details/gbseqaucr.sHtML

[U54] PHP：空安全调用
来源：http://read.share.vehdjk.com/Article/details/gdbamxjtt.sHtML

$obj?->method()
来源：http://www.share.bbcook.cn/Article/details/gdgafhqyg.sHtML

[U55] PHP：match 表达式
来源：http://mobile.bbcook.cn/Article/details/gpjrnblfg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.epnwcf.com/Article/details/gcdnwswef.sHtML

[U56] PHP：命名参数
来源：http://wap.fktsv.cn/Article/details/gfpfzxxcj.sHtML

f(a: 1, b: 2)
来源：http://baike.bbcook.cn/Article/details/gkoehryrm.sHtML

[U57] PHP：字符串插值
来源：http://www.share.bbcook.cn/Article/details/gfmgrqcwe.sHtML

"值: {$a}"
来源：http://www.m.share.bbcook.cn/Article/details/gstwfurvv.sHtML

[U58] PHP：数组三件套
来源：http://mobile.epnwcf.com/Article/details/gjoomiqzf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.vehdjk.com/Article/details/gbsnxunmn.sHtML

[U59] PHP：自定义排序
来源：http://wap.yfazqb.com/Article/details/gnillwpon.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fktsv.cn/Article/details/gydwbrtph.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.epnwcf.com/Article/details/gvcyhjsyv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.bbcook.cn/Article/details/gijkaejtj.sHtML

[U61] PHP：正则
来源：http://baike.yfazqb.com/Article/details/guicwlnkl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.tarul.cn/Article/details/ghobdszdt.sHtML

[U62] PHP：日期对象
来源：http://www.share.epnwcf.com/Article/details/gqaytposf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.sjlbkw.cn/Article/details/gfqiboqqj.sHtML

[U63] PHP：文件读写
来源：http://m.share.vehdjk.com/Article/details/ggxknibet.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.epnwcf.com/Article/details/glfxptnnb.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.vehdjk.com/Article/details/gzvjsojqr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fktsv.cn/Article/details/gdjeizbxh.sHtML

[U65] PHP：会话
来源：http://mobile.bbcook.cn/Article/details/gbmbpugfj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gmmynnakd.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.yfazqb.com/Article/details/ggbdtdbym.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gvlxojgqj.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.tarul.cn/Article/details/gjoxhjhnj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.vehdjk.com/Article/details/golciviwl.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.sjlbkw.cn/Article/details/gwvagoyrk.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.epnwcf.com/Article/details/gwrfeducb.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fktsv.cn/Article/details/gllidtgvf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.bbcook.cn/Article/details/gmhhqfeyr.sHtML

[U70] PHP：PDO 事务
来源：http://3g.yfazqb.com/Article/details/gdxcyfune.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.tarul.cn/Article/details/gxqojhdcb.sHtML

[U71] PHP：抛出异常
来源：http://m.share.tarul.cn/Article/details/grsbxvnao.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.yfazqb.com/Article/details/gdsjikcmj.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fktsv.cn/Article/details/gkgeuabeq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fktsv.cn/Article/details/gldkqagbq.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.tarul.cn/Article/details/geqthpzvx.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.sjlbkw.cn/Article/details/giwxmxcja.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fktsv.cn/Article/details/gqhwvillm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.epnwcf.com/Article/details/gipwxlgid.sHtML

[U75] PHP：依赖注入
来源：http://3g.tarul.cn/Article/details/gzwapgxri.sHtML

composer require psr/container
来源：http://mobile.sjlbkw.cn/Article/details/gtkmfarsq.sHtML

[U76] PHP：简单路由
来源：http://read.share.sjlbkw.cn/Article/details/gazeandwv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.yfazqb.com/Article/details/gdsglmehz.sHtML

[U77] PHP：模板渲染
来源：http://3g.bbcook.cn/Article/details/gngnggnwt.sHtML

composer require twig/twig
来源：http://mobile.tarul.cn/Article/details/gjrunbfvr.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fktsv.cn/Article/details/gmxorpweu.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.epnwcf.com/Article/details/gsukofwab.sHtML

[U79] PHP：静态分析
来源：http://wap.bbcook.cn/Article/details/gcpiriakj.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.tarul.cn/Article/details/gzvtskhgl.sHtML

[U80] PHP：代码规范修复
来源：http://wap.yfazqb.com/Article/details/gwahuniox.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.yfazqb.com/Article/details/gxwbrsszv.sHtML

[U81] JS：初始化项目
来源：http://3g.yfazqb.com/Article/details/gwmyxtspr.sHtML

npm init -y;  npm i express
来源：http://www.blog.sjlbkw.cn/Article/details/gansqcxpy.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.tarul.cn/Article/details/gtbfffdgv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.yfazqb.com/Article/details/gjsmjzqeg.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.bbcook.cn/Article/details/gmhjgyiko.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.yfazqb.com/Article/details/gnaglynzo.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.bbcook.cn/Article/details/gzleautps.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fktsv.cn/Article/details/guydljftc.sHtML

[U85] JS：可选链
来源：http://baike.bbcook.cn/Article/details/gxduwauzi.sHtML

a?.b?.c
来源：http://read.share.tarul.cn/Article/details/gdggeslvs.sHtML

[U86] JS：空值合并
来源：http://read.share.tarul.cn/Article/details/gdgdfketi.sHtML

a ?? b
来源：http://mobile.yfazqb.com/Article/details/gsleggzzw.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.sjlbkw.cn/Article/details/gkizqehem.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.vehdjk.com/Article/details/gxpyaovxb.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fktsv.cn/Article/details/gychejfrg.sHtML

{ ...a, ...b }
来源：http://www.share.fktsv.cn/Article/details/gtkcabucj.sHtML

[U89] JS：数组去重
来源：http://www.blog.tarul.cn/Article/details/gulqsxsii.sHtML

[...new Set(arr)]
来源：http://www.blog.yfazqb.com/Article/details/gbrjhhkqk.sHtML

[U90] JS：数字数组排序
来源：http://3g.tarul.cn/Article/details/gihhqxpmh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.epnwcf.com/Article/details/gakmdqueh.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.bbcook.cn/Article/details/gqyyfykem.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.epnwcf.com/Article/details/gkgpecrhe.sHtML

[U92] JS：深拷贝
来源：http://baike.yfazqb.com/Article/details/geqibbrkc.sHtML

structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/gvwkycavh.sHtML

[U93] JS：模板字符串
来源：http://blog.bbcook.cn/Article/details/gnzewwbax.sHtML

`共 ${n} 条`
来源：http://www.m.share.tarul.cn/Article/details/gujhtugrm.sHtML

[U94] JS：箭头函数
来源：http://read.share.vehdjk.com/Article/details/gqzkwprix.sHtML

const double = x => x * 2;
来源：http://read.share.epnwcf.com/Article/details/gqwwhmrip.sHtML

[U95] JS：Promise 包装
来源：http://read.share.bbcook.cn/Article/details/girdxinoj.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.bbcook.cn/Article/details/gvlojziqp.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.epnwcf.com/Article/details/gcfsscvtp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.tarul.cn/Article/details/gchodadxf.sHtML

[U97] JS：并发请求
来源：http://mobile.sjlbkw.cn/Article/details/gzzzkfhbl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/gxvcfclcr.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.bbcook.cn/Article/details/gaowwzwau.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.vehdjk.com/Article/details/gnlzfmnog.sHtML

[U99] JS：事件监听
来源：http://baike.epnwcf.com/Article/details/gmgmqsycr.sHtML

el.addEventListener("click", e => {})
来源：http://blog.sjlbkw.cn/Article/details/ghpightof.sHtML

[U100] JS：DOM 查询
来源：http://3g.sjlbkw.cn/Article/details/gwvhhlbmq.sHtML

document.querySelector(".item")
来源：http://3g.bbcook.cn/Article/details/gglccpsiz.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.yfazqb.com/Article/details/gduosxcqk.sHtML

el.classList.toggle("active")
来源：http://3g.fktsv.cn/Article/details/gxkebghqr.sHtML

[U102] JS：本地存储
来源：http://baike.bbcook.cn/Article/details/gaetrojvr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.sjlbkw.cn/Article/details/glngnvxgh.sHtML

[U103] JS：定时器
来源：http://blog.tarul.cn/Article/details/gbmedsktq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fktsv.cn/Article/details/gdysncxaj.sHtML

[U104] JS：防抖
来源：http://blog.epnwcf.com/Article/details/gjshzogbl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.tarul.cn/Article/details/guksqumwx.sHtML

[U105] JS：节流
来源：http://read.share.epnwcf.com/Article/details/gghittvtl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.bbcook.cn/Article/details/gorhomuvh.sHtML

[U106] JS：日期格式化
来源：http://www.blog.tarul.cn/Article/details/gmhpgpfjv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.sjlbkw.cn/Article/details/gvnaadbvu.sHtML

[U107] JS：数字千分位
来源：http://baike.yfazqb.com/Article/details/gmjaepcqz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.yfazqb.com/Article/details/gmuoytazn.sHtML

[U108] JS：随机整数
来源：http://m.share.vehdjk.com/Article/details/glszgjjhv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fktsv.cn/Article/details/gmjekstwf.sHtML

[U109] JS：数组分组
来源：http://www.share.vehdjk.com/Article/details/gdvzmhiut.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.sjlbkw.cn/Article/details/gouhsaycj.sHtML

[U110] JS：数组分块
来源：http://www.share.tarul.cn/Article/details/gbofslqlk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.vehdjk.com/Article/details/govkzdgbl.sHtML

[U111] JS：对象转 Map
来源：http://www.share.bbcook.cn/Article/details/gmqquizxu.sHtML

new Map(Object.entries(obj))
来源：http://wap.fktsv.cn/Article/details/gxcpmrirb.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fktsv.cn/Article/details/guwwhwkav.sHtML

"7".padStart(3, "0")
来源：http://www.share.yfazqb.com/Article/details/glquifghv.sHtML

[U113] JS：正则替换全部
来源：http://blog.tarul.cn/Article/details/gsyhpvfoj.sHtML

s.replaceAll("a", "b")
来源：http://wap.bbcook.cn/Article/details/gonrxhhux.sHtML

[U114] JS：JSON 深比较
来源：http://blog.vehdjk.com/Article/details/grkfhekxf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.bbcook.cn/Article/details/gtfwvjkkz.sHtML

[U115] JS：生成 UUID
来源：http://m.share.yfazqb.com/Article/details/gaaojmdxx.sHtML

crypto.randomUUID()
来源：http://blog.yfazqb.com/Article/details/grpxvmeel.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.bbcook.cn/Article/details/gwojhvyga.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.yfazqb.com/Article/details/ggsoguhja.sHtML

[U117] JS：单元测试
来源：http://www.blog.bbcook.cn/Article/details/gmmsawwtb.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.bbcook.cn/Article/details/gezwtarkn.sHtML

[U118] JS：开发服务器
来源：http://baike.bbcook.cn/Article/details/gxxapvzdo.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fktsv.cn/Article/details/gkedasdal.sHtML

[U119] JS：生产构建
来源：http://www.blog.tarul.cn/Article/details/gbirskzoy.sHtML

npx vite build
来源：http://www.m.share.sjlbkw.cn/Article/details/gcivhurld.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.epnwcf.com/Article/details/gqvfzxnvj.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.sjlbkw.cn/Article/details/givihzhhl.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gjikwmkcs.sHtML

统计汇总
来源：http://www.m.share.yfazqb.com/Article/details/ghcbtyvdm.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/giivbjaae.sHtML

按语言统计（条）：
来源：http://m.share.fktsv.cn/Article/details/gztieuqbx.sHtML

Python ......... 252
来源：http://read.share.tarul.cn/Article/details/gyoqpnuhw.sHtML

PHP ............ 252
来源：http://baike.tarul.cn/Article/details/gxhrtirfe.sHtML

JavaScript ..... 252
来源：http://mobile.vehdjk.com/Article/details/gunrfncbe.sHtML

TypeScript ..... 212
来源：http://read.share.epnwcf.com/Article/details/gkyqxhtlc.sHtML

Java ........... 212
来源：http://www.blog.tarul.cn/Article/details/gmstwoxsq.sHtML

Go ............. 212
来源：http://www.blog.bbcook.cn/Article/details/gvaybpdqf.sHtML

Ruby ........... 212
来源：http://blog.bbcook.cn/Article/details/gwfcptfle.sHtML

C# ............. 212
来源：http://3g.tarul.cn/Article/details/gctxqpkdd.sHtML

C .............. 30
来源：http://m.share.tarul.cn/Article/details/giwcipfkz.sHtML

C++ ............ 30
来源：http://m.share.bbcook.cn/Article/details/gtjkrpsyf.sHtML

SQL ............ 90
来源：http://wap.sjlbkw.cn/Article/details/gvbljyljj.sHtML

Bash ........... 80
来源：http://www.share.bbcook.cn/Article/details/ghfelzmty.sHtML

Kotlin ......... 15
来源：http://www.m.share.yfazqb.com/Article/details/gbfnkdqaq.sHtML

Swift .......... 15
来源：http://m.share.bbcook.cn/Article/details/gvjonshps.sHtML

Lua ............ 10
来源：http://m.share.vehdjk.com/Article/details/gkygrlrzd.sHtML

Perl ........... 10
来源：http://blog.yfazqb.com/Article/details/gbqjarmkf.sHtML

Scala .......... 10
来源：http://wap.bbcook.cn/Article/details/geqcystzy.sHtML

------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/guawfnwqk.sHtML

合计 ........... 2106 条
来源：http://wap.vehdjk.com/Article/details/geotuuemy.sHtML

按章节统计：
来源：http://www.share.epnwcf.com/Article/details/geghmovjv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.vehdjk.com/Article/details/goedheixx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.epnwcf.com/Article/details/gwiparisy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.yfazqb.com/Article/details/gdywtrdgd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.bbcook.cn/Article/details/guwojyogj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.yfazqb.com/Article/details/gsbapsgvy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.epnwcf.com/Article/details/gfyeqyslr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.vehdjk.com/Article/details/gnvcdpqpf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.sjlbkw.cn/Article/details/gkjvdzwlp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.epnwcf.com/Article/details/gvbcpqmdk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.epnwcf.com/Article/details/gpzmbjnxf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.bbcook.cn/Article/details/ggjzgbhfi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fktsv.cn/Article/details/galdwbufv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/gupudxlve.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.bbcook.cn/Article/details/gqtybzywy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.sjlbkw.cn/Article/details/gecsgoxwr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/giyscufrg.sHtML

Q SQL 专题                              90
来源：http://blog.fktsv.cn/Article/details/gbruqzcoy.sHtML

R Bash 专题                             80
来源：http://mobile.sjlbkw.cn/Article/details/gkuzeaqpe.sHtML

S C / C++ 专题                          60
来源：http://blog.tarul.cn/Article/details/grcadsyjw.sHtML

T 其他语言补充                          60
来源：http://www.blog.bbcook.cn/Article/details/gwpmqbvjg.sHtML

U 高频实用片段                         120
来源：http://baike.epnwcf.com/Article/details/gabrmhexm.sHtML

------------------------------------
来源：http://read.share.epnwcf.com/Article/details/gwdxrtsgg.sHtML

合计                                  2106 条
来源：http://m.share.yfazqb.com/Article/details/gajlbtkbm.sHtML

--------------------------------------------------------------------------------
来源：http://wap.vehdjk.com/Article/details/ggxofptyi.sHtML

使用提醒
来源：http://blog.tarul.cn/Article/details/gqadfkkkf.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.tarul.cn/Article/details/gpvfgtckn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.epnwcf.com/Article/details/gumwwldae.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.epnwcf.com/Article/details/gcjskwubb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.bbcook.cn/Article/details/gbeogeing.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.epnwcf.com/Article/details/ggzkdgyzq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.vehdjk.com/Article/details/gcgyvorhl.sHtML

—— 文件结束 ——
来源：http://www.blog.bbcook.cn/Article/details/gdaepncga.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gdvwxoqfq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.epnwcf.com/Article/details/gqxcqxnqg.sHtML

Common Programming Examples Cheat Book
来源：http://baike.yfazqb.com/Article/details/gtgagswre.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gebfgzfzu.sHtML

【收录内容】
来源：http://read.share.sjlbkw.cn/Article/details/gmogwawqx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.tarul.cn/Article/details/gvhunidsw.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.sjlbkw.cn/Article/details/gfyfrbddb.sHtML

SQL · Bash · C · C++
来源：http://www.share.vehdjk.com/Article/details/gqjvkpwfr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.epnwcf.com/Article/details/gzortlakm.sHtML

【使用说明】
来源：http://www.m.share.epnwcf.com/Article/details/ghgphgxrx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.tarul.cn/Article/details/groaoxehe.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.yfazqb.com/Article/details/gmmgtctif.sHtML


<!-- 参考信息 -->