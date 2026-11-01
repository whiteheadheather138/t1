代发 wailian999

[U07] Py：反转字典键值
来源：http://read.share.fktsv.cn/Article/details/gjxtrtcwu.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.tarul.cn/Article/details/gwgmzzxnt.sHtML

[U08] Py：展平二维列表
来源：http://www.blog.tarul.cn/Article/details/gzxpfzqkf.sHtML

[y for x in nested for y in x]
来源：http://www.blog.bbcook.cn/Article/details/govyjguhb.sHtML

[U09] Py：字典取最大值的键
来源：http://www.m.share.vehdjk.com/Article/details/gezlurvud.sHtML

max(d, key=d.get)
来源：http://www.share.tarul.cn/Article/details/gghdajorx.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.yfazqb.com/Article/details/giclimkkg.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.yfazqb.com/Article/details/ggylnnwcx.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgudiewd.sHtML

(x * 2 for x in arr)
来源：http://3g.vehdjk.com/Article/details/gsyysbcnm.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.vehdjk.com/Article/details/gwuzddxxp.sHtML

Counter(arr).most_common(3)
来源：http://read.share.epnwcf.com/Article/details/gcyhfxeik.sHtML

[U13] Py：固定长度队列
来源：http://www.share.yfazqb.com/Article/details/gbphqymcm.sHtML

deque(maxlen=10)
来源：http://3g.bbcook.cn/Article/details/gngrtffly.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.bbcook.cn/Article/details/ggkogkohl.sHtML

defaultdict(list)
来源：http://baike.bbcook.cn/Article/details/gyncrywsl.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.bbcook.cn/Article/details/gymvmevoe.sHtML

t = time.perf_counter()
来源：http://blog.epnwcf.com/Article/details/gvxkancir.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.sjlbkw.cn/Article/details/gggibpvtm.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.vehdjk.com/Article/details/gmvlwvmmi.sHtML

[U17] Py：初始化日志
来源：http://read.share.epnwcf.com/Article/details/gsalwdyhu.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.fktsv.cn/Article/details/gdanjnjsb.sHtML

[U18] Py：预编译正则
来源：http://mobile.fktsv.cn/Article/details/gbwpxameo.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.tarul.cn/Article/details/ggcvpztlq.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.bbcook.cn/Article/details/gzzttuajv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.fktsv.cn/Article/details/gtgojxhtx.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.fktsv.cn/Article/details/gkcvaswwu.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.yfazqb.com/Article/details/gzywdppiu.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.vehdjk.com/Article/details/gbvmvbmxy.sHtML

@contextlib.contextmanager
来源：http://wap.epnwcf.com/Article/details/gemdlwxtq.sHtML

[U22] Py：矩阵转置
来源：http://read.share.yfazqb.com/Article/details/gywihwhpy.sHtML

list(zip(*m))
来源：http://www.share.sjlbkw.cn/Article/details/gvwoinidd.sHtML

[U23] Py：分块读取大文件
来源：http://blog.bbcook.cn/Article/details/gooqggwby.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.bbcook.cn/Article/details/gfcuovlhq.sHtML

[U24] Py：路径操作
来源：http://www.blog.bbcook.cn/Article/details/gmbyulxlh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.bbcook.cn/Article/details/gmwowjaun.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.vehdjk.com/Article/details/gfuqojvpa.sHtML

csv.DictReader(f)
来源：http://www.share.yfazqb.com/Article/details/gcrxrprrb.sHtML

[U26] Py：并发下载
来源：http://wap.epnwcf.com/Article/details/gkghvfbzq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.fktsv.cn/Article/details/giwezlqxu.sHtML

[U27] Py：异步 HTTP
来源：http://3g.vehdjk.com/Article/details/gytiohobz.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.sjlbkw.cn/Article/details/ganwkeryv.sHtML

[U28] Py：类型别名
来源：http://blog.vehdjk.com/Article/details/giylnnpeo.sHtML

UserId = int
来源：http://mobile.sjlbkw.cn/Article/details/gniartahu.sHtML

[U29] Py：属性校验
来源：http://www.m.share.epnwcf.com/Article/details/gixlvvggh.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.bbcook.cn/Article/details/gqaacwhtg.sHtML

[U30] Py：数据类
来源：http://www.blog.tarul.cn/Article/details/gfbskgynl.sHtML

@dataclass(slots=True)
来源：http://mobile.vehdjk.com/Article/details/gvjkxrkkj.sHtML

[U31] Py：单测
来源：http://www.m.share.sjlbkw.cn/Article/details/gulgqnfhs.sHtML

python -m pytest -q
来源：http://www.m.share.bbcook.cn/Article/details/gbhikciae.sHtML

[U32] Py：代码格式化
来源：http://www.share.tarul.cn/Article/details/gffrbhvnr.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.yfazqb.com/Article/details/gowlfbqto.sHtML

[U33] Py：打包发布
来源：http://baike.yfazqb.com/Article/details/giubrygam.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.sjlbkw.cn/Article/details/gixpazwym.sHtML

[U34] Py：判断编码
来源：http://www.share.tarul.cn/Article/details/gecoqbxib.sHtML

chardet.detect(raw)
来源：http://www.m.share.tarul.cn/Article/details/gbvaqumxt.sHtML

[U35] Py：发送邮件
来源：http://www.share.fktsv.cn/Article/details/gmrmgurgj.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.vehdjk.com/Article/details/gzywwloak.sHtML

[U36] Py：定时任务
来源：http://3g.bbcook.cn/Article/details/gjbtnwuzv.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.sjlbkw.cn/Article/details/giptkyqgd.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.tarul.cn/Article/details/glxwzlsia.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.tarul.cn/Article/details/gbevukkjc.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.sjlbkw.cn/Article/details/gwnrjzvhq.sHtML

Path(__file__).resolve().parent
来源：http://mobile.tarul.cn/Article/details/gbfhwarmf.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.sjlbkw.cn/Article/details/gtgxntavc.sHtML

sys.stdout.isatty()
来源：http://m.share.bbcook.cn/Article/details/gyqnjgqrk.sHtML

[U40] Py：打印到标准错误
来源：http://blog.yfazqb.com/Article/details/gaqnbapii.sHtML

print("err", file=sys.stderr)
来源：http://mobile.epnwcf.com/Article/details/gfwhywrhs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.blog.tarul.cn/Article/details/gmecigfqf.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.fktsv.cn/Article/details/gmanwjvkq.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.tarul.cn/Article/details/guyaheyku.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.sjlbkw.cn/Article/details/glklqzvdo.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdoaeewt.sHtML

namespace App\Http;
来源：http://mobile.tarul.cn/Article/details/gbngbkdrw.sHtML

[U44] PHP：开启严格类型
来源：http://3g.bbcook.cn/Article/details/ghvxcqqlx.sHtML

declare(strict_types=1);
来源：http://blog.sjlbkw.cn/Article/details/gvikipcjt.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.fktsv.cn/Article/details/gnwgwhepz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.vehdjk.com/Article/details/gzftbiuoe.sHtML

[U46] PHP：可空类型
来源：http://blog.fktsv.cn/Article/details/glahuxchj.sHtML

?string $name = null
来源：http://baike.bbcook.cn/Article/details/gvsusevxi.sHtML

[U47] PHP：联合类型
来源：http://baike.bbcook.cn/Article/details/gwbjatcas.sHtML

int|string $id
来源：http://mobile.sjlbkw.cn/Article/details/ggzhcxlms.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.vehdjk.com/Article/details/gnkkefbpk.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.fktsv.cn/Article/details/gmhgriuac.sHtML

[U49] PHP：只读属性
来源：http://3g.yfazqb.com/Article/details/ggjzlsycy.sHtML

public readonly string $name
来源：http://www.blog.epnwcf.com/Article/details/gzbvmlymq.sHtML

[U50] PHP：构造器属性提升
来源：http://read.share.bbcook.cn/Article/details/glqbgermw.sHtML

public function __construct(private int $id) {}
来源：http://blog.epnwcf.com/Article/details/gzufzthym.sHtML

[U51] PHP：数组解构
来源：http://3g.bbcook.cn/Article/details/gzifbdoll.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.bbcook.cn/Article/details/gxjsjjfje.sHtML

[U52] PHP：箭头函数
来源：http://read.share.bbcook.cn/Article/details/gvejglkcd.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.bbcook.cn/Article/details/gdghxanhu.sHtML

[U53] PHP：空合并运算符
来源：http://baike.bbcook.cn/Article/details/gexmtvwmv.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.epnwcf.com/Article/details/gwnmqomkg.sHtML

[U54] PHP：空安全调用
来源：http://mobile.sjlbkw.cn/Article/details/gzqfqjfeh.sHtML

$obj?->method()
来源：http://wap.sjlbkw.cn/Article/details/gmetzcrdb.sHtML

[U55] PHP：match 表达式
来源：http://wap.fktsv.cn/Article/details/geqzptvsb.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.fktsv.cn/Article/details/guyxhipqh.sHtML

[U56] PHP：命名参数
来源：http://mobile.sjlbkw.cn/Article/details/guevrhgag.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.yfazqb.com/Article/details/gmbgrkqli.sHtML

[U57] PHP：字符串插值
来源：http://www.share.vehdjk.com/Article/details/gueeicrld.sHtML

"值: {$a}"
来源：http://mobile.vehdjk.com/Article/details/gtpnkriwn.sHtML

[U58] PHP：数组三件套
来源：http://read.share.yfazqb.com/Article/details/gigkeofwb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.yfazqb.com/Article/details/gxmleqbtg.sHtML

[U59] PHP：自定义排序
来源：http://mobile.bbcook.cn/Article/details/gllwxmefe.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.bbcook.cn/Article/details/ghcnbyrea.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.bbcook.cn/Article/details/gdyudkqie.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.epnwcf.com/Article/details/gigvotwqy.sHtML

[U61] PHP：正则
来源：http://www.blog.sjlbkw.cn/Article/details/gycwirqdt.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fktsv.cn/Article/details/gverpocaw.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.epnwcf.com/Article/details/gvjjoxzxj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.sjlbkw.cn/Article/details/gkadujdqd.sHtML

[U63] PHP：文件读写
来源：http://blog.tarul.cn/Article/details/gmtynnvlh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.sjlbkw.cn/Article/details/gedtgnagn.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.tarul.cn/Article/details/gdkfqnclq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.epnwcf.com/Article/details/gdnadntri.sHtML

[U65] PHP：会话
来源：http://blog.fktsv.cn/Article/details/gxfgjixpb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.tarul.cn/Article/details/gducjcruz.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.bbcook.cn/Article/details/gmbfijhpz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.bbcook.cn/Article/details/gzevxjwzd.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.sjlbkw.cn/Article/details/gcwhmulgv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.vehdjk.com/Article/details/gxgclwccf.sHtML

[U68] PHP：PDO 连接
来源：http://baike.tarul.cn/Article/details/gwqcxezvt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.tarul.cn/Article/details/gwdktavnh.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.sjlbkw.cn/Article/details/ggyesvxdm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fktsv.cn/Article/details/ggqmcwpia.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.sjlbkw.cn/Article/details/ghleofutx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.yfazqb.com/Article/details/gqivmhsns.sHtML

[U71] PHP：抛出异常
来源：http://blog.yfazqb.com/Article/details/ghulcbdic.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.tarul.cn/Article/details/gaheofmxt.sHtML

[U72] PHP：写错误日志
来源：http://read.share.sjlbkw.cn/Article/details/gwcyievcv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fktsv.cn/Article/details/gnysxdmxs.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.bbcook.cn/Article/details/ggepgaykg.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.epnwcf.com/Article/details/gipfzrzpu.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.epnwcf.com/Article/details/gellestym.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.tarul.cn/Article/details/gugwicvzr.sHtML

[U75] PHP：依赖注入
来源：http://www.share.tarul.cn/Article/details/gwtggbsob.sHtML

composer require psr/container
来源：http://read.share.yfazqb.com/Article/details/glpwbdxkd.sHtML

[U76] PHP：简单路由
来源：http://m.share.tarul.cn/Article/details/gcfhknhmr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.sjlbkw.cn/Article/details/gxqihwgwn.sHtML

[U77] PHP：模板渲染
来源：http://3g.epnwcf.com/Article/details/gbfjlidkm.sHtML

composer require twig/twig
来源：http://www.share.sjlbkw.cn/Article/details/gctyftmiu.sHtML

[U78] PHP：单元测试
来源：http://3g.epnwcf.com/Article/details/gtcjlxblm.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.yfazqb.com/Article/details/gwvhgqrgq.sHtML

[U79] PHP：静态分析
来源：http://baike.sjlbkw.cn/Article/details/gdqdghvgi.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.epnwcf.com/Article/details/gvqogcrbr.sHtML

[U80] PHP：代码规范修复
来源：http://baike.vehdjk.com/Article/details/gnngfbfui.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.yfazqb.com/Article/details/gtvumrsjw.sHtML

[U81] JS：初始化项目
来源：http://www.blog.sjlbkw.cn/Article/details/grwrhsgcj.sHtML

npm init -y;  npm i express
来源：http://read.share.fktsv.cn/Article/details/gxpqkcaoe.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.tarul.cn/Article/details/gtlijwtej.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.yfazqb.com/Article/details/gnlllzqaj.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.tarul.cn/Article/details/gjkpulcyo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.sjlbkw.cn/Article/details/gdsnumheg.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.yfazqb.com/Article/details/glqnebixh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.vehdjk.com/Article/details/gltppoiyx.sHtML

[U85] JS：可选链
来源：http://3g.epnwcf.com/Article/details/gxjcbqvzw.sHtML

a?.b?.c
来源：http://m.share.tarul.cn/Article/details/grjwxecat.sHtML

[U86] JS：空值合并
来源：http://www.blog.sjlbkw.cn/Article/details/gpjxobrmf.sHtML

a ?? b
来源：http://3g.yfazqb.com/Article/details/gycwzgain.sHtML

[U87] JS：解构默认值
来源：http://3g.sjlbkw.cn/Article/details/ghuwcehyx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.tarul.cn/Article/details/gbikiiuzd.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fktsv.cn/Article/details/grtggosid.sHtML

{ ...a, ...b }
来源：http://m.share.tarul.cn/Article/details/gzgndsdob.sHtML

[U89] JS：数组去重
来源：http://www.m.share.yfazqb.com/Article/details/grqzavpgj.sHtML

[...new Set(arr)]
来源：http://wap.vehdjk.com/Article/details/gbbgluxtd.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fktsv.cn/Article/details/gwhxcgenq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.yfazqb.com/Article/details/gsshzuuoo.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.tarul.cn/Article/details/gkjuhdvuz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.yfazqb.com/Article/details/grpykvzpc.sHtML

[U92] JS：深拷贝
来源：http://wap.bbcook.cn/Article/details/gufkpepqn.sHtML

structuredClone(obj)
来源：http://wap.tarul.cn/Article/details/gzarzsghg.sHtML

[U93] JS：模板字符串
来源：http://mobile.sjlbkw.cn/Article/details/gfrijarzh.sHtML

`共 ${n} 条`
来源：http://blog.vehdjk.com/Article/details/ggmcombqf.sHtML

[U94] JS：箭头函数
来源：http://blog.fktsv.cn/Article/details/gpieuynks.sHtML

const double = x => x * 2;
来源：http://www.share.sjlbkw.cn/Article/details/ggjkskydw.sHtML

[U95] JS：Promise 包装
来源：http://m.share.epnwcf.com/Article/details/gsozejqqh.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.yfazqb.com/Article/details/ghnxmtign.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fktsv.cn/Article/details/gfevvkxtw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.bbcook.cn/Article/details/gaqlgdukn.sHtML

[U97] JS：并发请求
来源：http://3g.epnwcf.com/Article/details/gdgylgrrx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fktsv.cn/Article/details/gjkxlsdow.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.tarul.cn/Article/details/gxnvbtgmy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.epnwcf.com/Article/details/gxzfxcgrn.sHtML

[U99] JS：事件监听
来源：http://www.blog.fktsv.cn/Article/details/gpeafoxrb.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fktsv.cn/Article/details/gpblbmhos.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fktsv.cn/Article/details/gklebpfuj.sHtML

document.querySelector(".item")
来源：http://blog.fktsv.cn/Article/details/giudqkxar.sHtML

[U101] JS：classList 操作
来源：http://read.share.fktsv.cn/Article/details/gsvkrjmsr.sHtML

el.classList.toggle("active")
来源：http://www.share.vehdjk.com/Article/details/ggmlbjtbb.sHtML

[U102] JS：本地存储
来源：http://wap.vehdjk.com/Article/details/gzeflkqfc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.sjlbkw.cn/Article/details/gxdrewfyq.sHtML

[U103] JS：定时器
来源：http://blog.epnwcf.com/Article/details/geaabuqos.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.epnwcf.com/Article/details/gqqebfonw.sHtML

[U104] JS：防抖
来源：http://baike.fktsv.cn/Article/details/gilnpjxdb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.sjlbkw.cn/Article/details/gmfodksbs.sHtML

[U105] JS：节流
来源：http://blog.fktsv.cn/Article/details/gwxgqeaaa.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.vehdjk.com/Article/details/gvvsouhpt.sHtML

[U106] JS：日期格式化
来源：http://3g.sjlbkw.cn/Article/details/gnimajrmj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.yfazqb.com/Article/details/givchxzka.sHtML

[U107] JS：数字千分位
来源：http://mobile.fktsv.cn/Article/details/gmnmdmtel.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.bbcook.cn/Article/details/gjztzuczd.sHtML

[U108] JS：随机整数
来源：http://www.m.share.epnwcf.com/Article/details/gxrvmhhss.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.tarul.cn/Article/details/gcekixjit.sHtML

[U109] JS：数组分组
来源：http://wap.bbcook.cn/Article/details/gkfwlbjio.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.epnwcf.com/Article/details/gfkpsvixr.sHtML

[U110] JS：数组分块
来源：http://m.share.sjlbkw.cn/Article/details/grfjsuiuv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.sjlbkw.cn/Article/details/gimlqbogx.sHtML

[U111] JS：对象转 Map
来源：http://read.share.epnwcf.com/Article/details/ggqhdntus.sHtML

new Map(Object.entries(obj))
来源：http://m.share.bbcook.cn/Article/details/gqmclaqeu.sHtML

[U112] JS：字符串补位
来源：http://read.share.sjlbkw.cn/Article/details/gchyfqhch.sHtML

"7".padStart(3, "0")
来源：http://m.share.yfazqb.com/Article/details/ghtedzxyl.sHtML

[U113] JS：正则替换全部
来源：http://www.share.vehdjk.com/Article/details/gmqvxucxh.sHtML

s.replaceAll("a", "b")
来源：http://blog.sjlbkw.cn/Article/details/gbgyymyfp.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.vehdjk.com/Article/details/ggffdyuzj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.vehdjk.com/Article/details/gaqvaonhv.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fktsv.cn/Article/details/gjafrqzai.sHtML

crypto.randomUUID()
来源：http://blog.tarul.cn/Article/details/gcdokekyv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fktsv.cn/Article/details/gbxnccxnr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fktsv.cn/Article/details/ghybkabzo.sHtML

[U117] JS：单元测试
来源：http://www.blog.epnwcf.com/Article/details/gatirtlfp.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.yfazqb.com/Article/details/giigfqtnr.sHtML

[U118] JS：开发服务器
来源：http://baike.tarul.cn/Article/details/ggozrslvx.sHtML

npm i -D vite;  npx vite
来源：http://mobile.epnwcf.com/Article/details/gmrpdcwlb.sHtML

[U119] JS：生产构建
来源：http://blog.bbcook.cn/Article/details/gdbinwqjz.sHtML

npx vite build
来源：http://www.share.fktsv.cn/Article/details/gbnqvexcu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.epnwcf.com/Article/details/gcffoxktr.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.tarul.cn/Article/details/gxpnwiaiy.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gsvgvzhnf.sHtML

统计汇总
来源：http://blog.tarul.cn/Article/details/gkztctdmc.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gcrvxbjoj.sHtML

按语言统计（条）：
来源：http://blog.sjlbkw.cn/Article/details/gsyofyawq.sHtML

Python ......... 252
来源：http://mobile.yfazqb.com/Article/details/gdezfxujx.sHtML

PHP ............ 252
来源：http://m.share.fktsv.cn/Article/details/gebwecmgv.sHtML

JavaScript ..... 252
来源：http://3g.sjlbkw.cn/Article/details/gtbtqmghr.sHtML

TypeScript ..... 212
来源：http://www.share.bbcook.cn/Article/details/goxfcehla.sHtML

Java ........... 212
来源：http://mobile.bbcook.cn/Article/details/ghojuktks.sHtML

Go ............. 212
来源：http://3g.sjlbkw.cn/Article/details/gsadfmymv.sHtML

Ruby ........... 212
来源：http://www.share.tarul.cn/Article/details/gdnlxwrbg.sHtML

C# ............. 212
来源：http://www.blog.yfazqb.com/Article/details/gnnvwpiyq.sHtML

C .............. 30
来源：http://baike.epnwcf.com/Article/details/ggczygifq.sHtML

C++ ............ 30
来源：http://baike.fktsv.cn/Article/details/gfiqffuvk.sHtML

SQL ............ 90
来源：http://mobile.vehdjk.com/Article/details/gzzofuikt.sHtML

Bash ........... 80
来源：http://3g.epnwcf.com/Article/details/gdyahsoaa.sHtML

Kotlin ......... 15
来源：http://3g.yfazqb.com/Article/details/gfwoicbxw.sHtML

Swift .......... 15
来源：http://mobile.epnwcf.com/Article/details/grhwrlncj.sHtML

Lua ............ 10
来源：http://blog.sjlbkw.cn/Article/details/ghlohxgrc.sHtML

Perl ........... 10
来源：http://3g.yfazqb.com/Article/details/gbwfybept.sHtML

Scala .......... 10
来源：http://3g.tarul.cn/Article/details/gmkqhgftg.sHtML

------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gmeruhgio.sHtML

合计 ........... 2106 条
来源：http://wap.yfazqb.com/Article/details/gpgrtdrld.sHtML

按章节统计：
来源：http://www.blog.vehdjk.com/Article/details/gnriupgdf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.sjlbkw.cn/Article/details/ghebtckby.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.bbcook.cn/Article/details/gjglmloiu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.bbcook.cn/Article/details/gxuulgnux.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fktsv.cn/Article/details/gwjvseffq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.epnwcf.com/Article/details/gemeidvoy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.bbcook.cn/Article/details/gxuwswyda.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fktsv.cn/Article/details/gdwcmyvcl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fktsv.cn/Article/details/gynvatsqy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/gatkyrsut.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fktsv.cn/Article/details/gzlwvfsgo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.tarul.cn/Article/details/gszgwitxo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fktsv.cn/Article/details/gpivnuccv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gbwjlkbqg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.epnwcf.com/Article/details/gxsdzmqfu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.epnwcf.com/Article/details/gckgznvvj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/gaufhvodh.sHtML

Q SQL 专题                              90
来源：http://www.m.share.bbcook.cn/Article/details/gelnftsts.sHtML

R Bash 专题                             80
来源：http://m.share.tarul.cn/Article/details/glbjztofw.sHtML

S C / C++ 专题                          60
来源：http://read.share.epnwcf.com/Article/details/ggkombbgp.sHtML

T 其他语言补充                          60
来源：http://www.blog.vehdjk.com/Article/details/genztnanc.sHtML

U 高频实用片段                         120
来源：http://www.m.share.yfazqb.com/Article/details/gqxxneklw.sHtML

------------------------------------
来源：http://3g.epnwcf.com/Article/details/gxwincwqd.sHtML

合计                                  2106 条
来源：http://blog.epnwcf.com/Article/details/glbarjhrj.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.epnwcf.com/Article/details/gywoepgdr.sHtML

使用提醒
来源：http://wap.sjlbkw.cn/Article/details/glheocfgz.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.yfazqb.com/Article/details/gastntujq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.epnwcf.com/Article/details/gcrrcwkpi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.sjlbkw.cn/Article/details/gcjcpojag.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fktsv.cn/Article/details/gqxydfbto.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.yfazqb.com/Article/details/gtrgexjxd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.vehdjk.com/Article/details/gdxqeghvm.sHtML

—— 文件结束 ——
来源：http://wap.epnwcf.com/Article/details/gwncibetx.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gjnxwcfqf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fktsv.cn/Article/details/glknxlqla.sHtML

Common Programming Examples Cheat Book
来源：http://blog.epnwcf.com/Article/details/guahbctqc.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gyyhysgwv.sHtML

【收录内容】
来源：http://baike.sjlbkw.cn/Article/details/glcuxrbzn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.bbcook.cn/Article/details/gaqzveyek.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.vehdjk.com/Article/details/gskqgxvhp.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.bbcook.cn/Article/details/gliaczlzl.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.epnwcf.com/Article/details/gfgbnqknc.sHtML

【使用说明】
来源：http://www.m.share.vehdjk.com/Article/details/gymmxvxkk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.sjlbkw.cn/Article/details/gfukmrdfk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.tarul.cn/Article/details/glrdzlaqv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.bbcook.cn/Article/details/gioqwqqjk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxvaomzb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.bbcook.cn/Article/details/ghgasqfrs.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.yfazqb.com/Article/details/gvqdmqeus.sHtML


<!-- 参考信息 -->