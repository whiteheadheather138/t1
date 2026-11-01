代发 wailian999

[U05] Py：列表去重且保序
来源：http://wap.sjlbkw.cn/Article/details/gjixcpzie.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.fktsv.cn/Article/details/gsymlicpg.sHtML

[U06] Py：合并两个字典
来源：http://read.share.yfazqb.com/Article/details/gakxydglz.sHtML

{**a, **b}
来源：http://read.share.fktsv.cn/Article/details/gqqmhjruo.sHtML

[U07] Py：反转字典键值
来源：http://read.share.sjlbkw.cn/Article/details/gybelshkb.sHtML

{v: k for k, v in d.items()}
来源：http://baike.epnwcf.com/Article/details/gfsngpinx.sHtML

[U08] Py：展平二维列表
来源：http://m.share.epnwcf.com/Article/details/gfnutcagt.sHtML

[y for x in nested for y in x]
来源：http://read.share.bbcook.cn/Article/details/gvznymsva.sHtML

[U09] Py：字典取最大值的键
来源：http://3g.yfazqb.com/Article/details/gmkidrltj.sHtML

max(d, key=d.get)
来源：http://wap.tarul.cn/Article/details/gmurartpe.sHtML

[U10] Py：按值排序字典
来源：http://read.share.yfazqb.com/Article/details/gpdqvrjrr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.vehdjk.com/Article/details/gyhsyvndq.sHtML

[U11] Py：生成器表达式
来源：http://mobile.fktsv.cn/Article/details/gpthgsnpi.sHtML

(x * 2 for x in arr)
来源：http://baike.yfazqb.com/Article/details/gjajyqkze.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.epnwcf.com/Article/details/guppbzftm.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.epnwcf.com/Article/details/ghmjyyovd.sHtML

[U13] Py：固定长度队列
来源：http://m.share.epnwcf.com/Article/details/grkowapxl.sHtML

deque(maxlen=10)
来源：http://www.blog.epnwcf.com/Article/details/guhfbnmgs.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.epnwcf.com/Article/details/gzynyegxg.sHtML

defaultdict(list)
来源：http://www.share.vehdjk.com/Article/details/gpkniyfkc.sHtML

[U15] Py：高精度计时
来源：http://read.share.tarul.cn/Article/details/gxgxwukfr.sHtML

t = time.perf_counter()
来源：http://m.share.bbcook.cn/Article/details/gqemfebvc.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.epnwcf.com/Article/details/gezjixala.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.bbcook.cn/Article/details/gxfevcccp.sHtML

[U17] Py：初始化日志
来源：http://www.share.epnwcf.com/Article/details/gynvrbrxa.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.vehdjk.com/Article/details/gsythnhpc.sHtML

[U18] Py：预编译正则
来源：http://mobile.yfazqb.com/Article/details/gfnwoiwyp.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.sjlbkw.cn/Article/details/gmyzriccg.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.tarul.cn/Article/details/gcdanmnxs.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.sjlbkw.cn/Article/details/guawejaic.sHtML

[U20] Py：缓存函数结果
来源：http://wap.bbcook.cn/Article/details/gxvusnjwj.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.epnwcf.com/Article/details/grrajloof.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.fktsv.cn/Article/details/gdnmojhbf.sHtML

@contextlib.contextmanager
来源：http://mobile.epnwcf.com/Article/details/grgdaylkg.sHtML

[U22] Py：矩阵转置
来源：http://3g.epnwcf.com/Article/details/gmikkdixy.sHtML

list(zip(*m))
来源：http://wap.tarul.cn/Article/details/gtgpubyhf.sHtML

[U23] Py：分块读取大文件
来源：http://baike.epnwcf.com/Article/details/gjhrioacq.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.bbcook.cn/Article/details/gewbobeiw.sHtML

[U24] Py：路径操作
来源：http://mobile.tarul.cn/Article/details/gbggyjwzr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.vehdjk.com/Article/details/gclbkoifk.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.fktsv.cn/Article/details/gdcevrjww.sHtML

csv.DictReader(f)
来源：http://blog.epnwcf.com/Article/details/gnvrqfruk.sHtML

[U26] Py：并发下载
来源：http://baike.bbcook.cn/Article/details/ghlrdgdiq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.vehdjk.com/Article/details/gvfvafgwi.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.tarul.cn/Article/details/gsjsphrps.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.epnwcf.com/Article/details/gjlyccfho.sHtML

[U28] Py：类型别名
来源：http://m.share.epnwcf.com/Article/details/gsbfdmvdu.sHtML

UserId = int
来源：http://3g.tarul.cn/Article/details/gbodnilym.sHtML

[U29] Py：属性校验
来源：http://www.blog.fktsv.cn/Article/details/gyiwdijdq.sHtML

@property 与 @x.setter 配合
来源：http://m.share.bbcook.cn/Article/details/gymtvnrjh.sHtML

[U30] Py：数据类
来源：http://m.share.tarul.cn/Article/details/gdnbmeige.sHtML

@dataclass(slots=True)
来源：http://wap.bbcook.cn/Article/details/gqtddpitn.sHtML

[U31] Py：单测
来源：http://baike.bbcook.cn/Article/details/gafsvttvi.sHtML

python -m pytest -q
来源：http://blog.vehdjk.com/Article/details/gfgquezns.sHtML

[U32] Py：代码格式化
来源：http://blog.tarul.cn/Article/details/goiggfmra.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.sjlbkw.cn/Article/details/grjuzexsc.sHtML

[U33] Py：打包发布
来源：http://blog.vehdjk.com/Article/details/gsthvlnkk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.epnwcf.com/Article/details/glytcqjlw.sHtML

[U34] Py：判断编码
来源：http://www.blog.epnwcf.com/Article/details/gttwnoxok.sHtML

chardet.detect(raw)
来源：http://wap.tarul.cn/Article/details/gdmmbdqev.sHtML

[U35] Py：发送邮件
来源：http://mobile.epnwcf.com/Article/details/gtggumhfi.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.sjlbkw.cn/Article/details/gttfdipbb.sHtML

[U36] Py：定时任务
来源：http://www.blog.yfazqb.com/Article/details/gnguglyeb.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.vehdjk.com/Article/details/giohewjup.sHtML

[U37] Py：读写 Excel
来源：http://mobile.yfazqb.com/Article/details/gjuzxoykm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.epnwcf.com/Article/details/gkzumaehj.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.epnwcf.com/Article/details/gjxqnafpc.sHtML

Path(__file__).resolve().parent
来源：http://www.share.yfazqb.com/Article/details/guwvlaitn.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.sjlbkw.cn/Article/details/gbgxczpsb.sHtML

sys.stdout.isatty()
来源：http://mobile.sjlbkw.cn/Article/details/gpxbwtiza.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.vehdjk.com/Article/details/gigarywhb.sHtML

print("err", file=sys.stderr)
来源：http://wap.tarul.cn/Article/details/gngzwplcs.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.vehdjk.com/Article/details/gqxbdlusx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.vehdjk.com/Article/details/gdhsldkjz.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.m.share.fktsv.cn/Article/details/gnuvwojru.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.tarul.cn/Article/details/ggzqulzvb.sHtML

[U43] PHP：声明命名空间
来源：http://baike.tarul.cn/Article/details/gsvxyukcw.sHtML

namespace App\Http;
来源：http://blog.epnwcf.com/Article/details/glllpmixv.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.fktsv.cn/Article/details/gnrpupmmh.sHtML

declare(strict_types=1);
来源：http://www.m.share.sjlbkw.cn/Article/details/gngnxeyuv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.vehdjk.com/Article/details/gzmpmjwkw.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.yfazqb.com/Article/details/gffujqzvy.sHtML

[U46] PHP：可空类型
来源：http://3g.yfazqb.com/Article/details/gcedkjsof.sHtML

?string $name = null
来源：http://baike.sjlbkw.cn/Article/details/gshxiqelv.sHtML

[U47] PHP：联合类型
来源：http://blog.tarul.cn/Article/details/gbilosksj.sHtML

int|string $id
来源：http://blog.epnwcf.com/Article/details/ghfhjgdpi.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.sjlbkw.cn/Article/details/gotbmcddn.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.yfazqb.com/Article/details/garulyagf.sHtML

[U49] PHP：只读属性
来源：http://3g.vehdjk.com/Article/details/gtbvqhgca.sHtML

public readonly string $name
来源：http://m.share.sjlbkw.cn/Article/details/gpukbgbdw.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.tarul.cn/Article/details/gtprgtzuk.sHtML

public function __construct(private int $id) {}
来源：http://www.share.bbcook.cn/Article/details/gvqubvmyv.sHtML

[U51] PHP：数组解构
来源：http://www.share.vehdjk.com/Article/details/ggyhwkvqi.sHtML

[$a, $b] = $arr;
来源：http://read.share.yfazqb.com/Article/details/gfcnzkzfv.sHtML

[U52] PHP：箭头函数
来源：http://www.share.epnwcf.com/Article/details/gkkpyzcgb.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.vehdjk.com/Article/details/gzurxdtmm.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.vehdjk.com/Article/details/gvtgdfdgj.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.sjlbkw.cn/Article/details/gmycinmyy.sHtML

[U54] PHP：空安全调用
来源：http://www.share.vehdjk.com/Article/details/gkmbecnrt.sHtML

$obj?->method()
来源：http://read.share.vehdjk.com/Article/details/grphhxldl.sHtML

[U55] PHP：match 表达式
来源：http://blog.tarul.cn/Article/details/glfwgmxbc.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fktsv.cn/Article/details/gedxjowkq.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.tarul.cn/Article/details/gozjjgmkv.sHtML

f(a: 1, b: 2)
来源：http://www.blog.epnwcf.com/Article/details/gswkteaim.sHtML

[U57] PHP：字符串插值
来源：http://mobile.epnwcf.com/Article/details/geddufjvr.sHtML

"值: {$a}"
来源：http://mobile.tarul.cn/Article/details/gnubsvmjx.sHtML

[U58] PHP：数组三件套
来源：http://wap.sjlbkw.cn/Article/details/gqlricyur.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.fktsv.cn/Article/details/giogyrwhr.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.epnwcf.com/Article/details/gshmsgwlr.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fktsv.cn/Article/details/gfzuwnbxz.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.yfazqb.com/Article/details/gantvgaxu.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.epnwcf.com/Article/details/glpkcbqkv.sHtML

[U61] PHP：正则
来源：http://blog.yfazqb.com/Article/details/glbvcmoir.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.sjlbkw.cn/Article/details/ghwrddsgn.sHtML

[U62] PHP：日期对象
来源：http://wap.yfazqb.com/Article/details/gkxajggzq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.vehdjk.com/Article/details/gzbtxhjxv.sHtML

[U63] PHP：文件读写
来源：http://3g.sjlbkw.cn/Article/details/ghdrbxrve.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.epnwcf.com/Article/details/gnziytxld.sHtML

[U64] PHP：目录遍历
来源：http://wap.fktsv.cn/Article/details/gtbaeyvuz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.epnwcf.com/Article/details/gslyvrvil.sHtML

[U65] PHP：会话
来源：http://blog.fktsv.cn/Article/details/glasucgbu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.fktsv.cn/Article/details/gwnkuzuaj.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.sjlbkw.cn/Article/details/gmdskints.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.sjlbkw.cn/Article/details/gfkewptky.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fktsv.cn/Article/details/ghrejgjmr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.sjlbkw.cn/Article/details/gevreeear.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.vehdjk.com/Article/details/gpwpsuyia.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.bbcook.cn/Article/details/gcmfvmqhc.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.vehdjk.com/Article/details/gcoybeflf.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.tarul.cn/Article/details/ggwijbvmp.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.fktsv.cn/Article/details/gybxdprha.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.sjlbkw.cn/Article/details/gnkcddxde.sHtML

[U71] PHP：抛出异常
来源：http://www.share.bbcook.cn/Article/details/gsvqjdkei.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.epnwcf.com/Article/details/grwuiprnu.sHtML

[U72] PHP：写错误日志
来源：http://baike.tarul.cn/Article/details/gnjxvaqle.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.fktsv.cn/Article/details/gvibpcefy.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.yfazqb.com/Article/details/guabcknbj.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.yfazqb.com/Article/details/grllpnzwu.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.bbcook.cn/Article/details/gbdugovpx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.epnwcf.com/Article/details/gqpnaukcu.sHtML

[U75] PHP：依赖注入
来源：http://baike.epnwcf.com/Article/details/gtisyyrrq.sHtML

composer require psr/container
来源：http://mobile.yfazqb.com/Article/details/ghohieegd.sHtML

[U76] PHP：简单路由
来源：http://blog.vehdjk.com/Article/details/glyltwzed.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.yfazqb.com/Article/details/gxctdhdzr.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.tarul.cn/Article/details/gbmxmolyx.sHtML

composer require twig/twig
来源：http://mobile.yfazqb.com/Article/details/gldzrtfyc.sHtML

[U78] PHP：单元测试
来源：http://baike.sjlbkw.cn/Article/details/gdijijwlh.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fktsv.cn/Article/details/gtaqfdsvj.sHtML

[U79] PHP：静态分析
来源：http://www.share.yfazqb.com/Article/details/ghawofaod.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.sjlbkw.cn/Article/details/gcqorohjp.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.vehdjk.com/Article/details/grqtufavi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.yfazqb.com/Article/details/gkhuiyuuq.sHtML

[U81] JS：初始化项目
来源：http://m.share.bbcook.cn/Article/details/gwfewadyb.sHtML

npm init -y;  npm i express
来源：http://3g.fktsv.cn/Article/details/gbyullfiw.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.vehdjk.com/Article/details/ghxcvagiw.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.tarul.cn/Article/details/gvipjulqr.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fktsv.cn/Article/details/gcjgmjxpt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.tarul.cn/Article/details/gqmascakr.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fktsv.cn/Article/details/gkrfrvfsb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.epnwcf.com/Article/details/gltowedqh.sHtML

[U85] JS：可选链
来源：http://read.share.tarul.cn/Article/details/gmcnennaq.sHtML

a?.b?.c
来源：http://read.share.bbcook.cn/Article/details/gmbhtjemd.sHtML

[U86] JS：空值合并
来源：http://read.share.sjlbkw.cn/Article/details/gcmgvjfyj.sHtML

a ?? b
来源：http://www.m.share.vehdjk.com/Article/details/gqiarwurl.sHtML

[U87] JS：解构默认值
来源：http://blog.tarul.cn/Article/details/gvytwvrnt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.vehdjk.com/Article/details/gnnmqotgk.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fktsv.cn/Article/details/gtukuegpz.sHtML

{ ...a, ...b }
来源：http://www.blog.sjlbkw.cn/Article/details/gdnslamvf.sHtML

[U89] JS：数组去重
来源：http://m.share.vehdjk.com/Article/details/gixdgbqal.sHtML

[...new Set(arr)]
来源：http://mobile.sjlbkw.cn/Article/details/gwhvogkvf.sHtML

[U90] JS：数字数组排序
来源：http://www.share.epnwcf.com/Article/details/gvfidcjjs.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.vehdjk.com/Article/details/gcfqeybvp.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fktsv.cn/Article/details/gpqnwrdsw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.vehdjk.com/Article/details/ggziicdyw.sHtML

[U92] JS：深拷贝
来源：http://baike.bbcook.cn/Article/details/goeqadyxa.sHtML

structuredClone(obj)
来源：http://wap.bbcook.cn/Article/details/grojtadxd.sHtML

[U93] JS：模板字符串
来源：http://read.share.vehdjk.com/Article/details/gjnmrjrfy.sHtML

`共 ${n} 条`
来源：http://m.share.epnwcf.com/Article/details/ghudzdymd.sHtML

[U94] JS：箭头函数
来源：http://www.blog.bbcook.cn/Article/details/gjyqbpaui.sHtML

const double = x => x * 2;
来源：http://read.share.epnwcf.com/Article/details/gjgmvjhte.sHtML

[U95] JS：Promise 包装
来源：http://baike.epnwcf.com/Article/details/gbdhtroyh.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fktsv.cn/Article/details/gwhpnttao.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdnakmmt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.vehdjk.com/Article/details/gzgrgwkzu.sHtML

[U97] JS：并发请求
来源：http://blog.sjlbkw.cn/Article/details/gtxtroqju.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/glemfukpn.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.bbcook.cn/Article/details/gyvgsovkk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fktsv.cn/Article/details/glmscbeab.sHtML

[U99] JS：事件监听
来源：http://read.share.tarul.cn/Article/details/guduoaagy.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.bbcook.cn/Article/details/gmyhwqkxx.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fktsv.cn/Article/details/gprrljkch.sHtML

document.querySelector(".item")
来源：http://wap.bbcook.cn/Article/details/gkjdovqta.sHtML

[U101] JS：classList 操作
来源：http://baike.fktsv.cn/Article/details/genfbjaby.sHtML

el.classList.toggle("active")
来源：http://m.share.tarul.cn/Article/details/guquepncd.sHtML

[U102] JS：本地存储
来源：http://baike.bbcook.cn/Article/details/gjdicoktf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.epnwcf.com/Article/details/gmkoszjvz.sHtML

[U103] JS：定时器
来源：http://baike.epnwcf.com/Article/details/gscfvkyqv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.tarul.cn/Article/details/gaqwymxba.sHtML

[U104] JS：防抖
来源：http://baike.tarul.cn/Article/details/gymcrvsyt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.sjlbkw.cn/Article/details/gqqjpcdfe.sHtML

[U105] JS：节流
来源：http://blog.fktsv.cn/Article/details/glcbjteqx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.bbcook.cn/Article/details/gvqmrklqn.sHtML

[U106] JS：日期格式化
来源：http://read.share.epnwcf.com/Article/details/gbdronnme.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.epnwcf.com/Article/details/gwqmoicrj.sHtML

[U107] JS：数字千分位
来源：http://read.share.epnwcf.com/Article/details/gobghzdsk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.sjlbkw.cn/Article/details/giezuybta.sHtML

[U108] JS：随机整数
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjufiedt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.vehdjk.com/Article/details/gzzcxynzh.sHtML

[U109] JS：数组分组
来源：http://3g.yfazqb.com/Article/details/gumczymcb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.sjlbkw.cn/Article/details/gstvhjrpq.sHtML

[U110] JS：数组分块
来源：http://m.share.bbcook.cn/Article/details/gdgpqmsxf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.sjlbkw.cn/Article/details/gnogjmqrd.sHtML

[U111] JS：对象转 Map
来源：http://baike.epnwcf.com/Article/details/gdlbihsss.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fktsv.cn/Article/details/gostrovde.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.bbcook.cn/Article/details/ghkmznfpk.sHtML

"7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/gcyljdnlz.sHtML

[U113] JS：正则替换全部
来源：http://www.share.yfazqb.com/Article/details/gjkewhxqz.sHtML

s.replaceAll("a", "b")
来源：http://3g.bbcook.cn/Article/details/gxoiswnnp.sHtML

[U114] JS：JSON 深比较
来源：http://blog.bbcook.cn/Article/details/gbuqkmbty.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.tarul.cn/Article/details/gtvctvyin.sHtML

[U115] JS：生成 UUID
来源：http://wap.bbcook.cn/Article/details/gwswaxhfk.sHtML

crypto.randomUUID()
来源：http://www.m.share.sjlbkw.cn/Article/details/gukdxdilj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.vehdjk.com/Article/details/gbebhpryt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fktsv.cn/Article/details/gjuihafym.sHtML

[U117] JS：单元测试
来源：http://blog.sjlbkw.cn/Article/details/gsmanlgby.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fktsv.cn/Article/details/gvatewplb.sHtML

[U118] JS：开发服务器
来源：http://baike.fktsv.cn/Article/details/grftotnht.sHtML

npm i -D vite;  npx vite
来源：http://baike.sjlbkw.cn/Article/details/gmhqjmezi.sHtML

[U119] JS：生产构建
来源：http://m.share.vehdjk.com/Article/details/ggxdnrksc.sHtML

npx vite build
来源：http://www.share.fktsv.cn/Article/details/gfzzxajfx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.yfazqb.com/Article/details/gwmyonyue.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fktsv.cn/Article/details/gvtxomjto.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ggqdfiywv.sHtML

统计汇总
来源：http://www.share.tarul.cn/Article/details/gnstqpksd.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gipddsnrg.sHtML

按语言统计（条）：
来源：http://3g.tarul.cn/Article/details/gdoydjsog.sHtML

Python ......... 252
来源：http://www.blog.bbcook.cn/Article/details/gbxqixpsl.sHtML

PHP ............ 252
来源：http://wap.sjlbkw.cn/Article/details/gnhmumebn.sHtML

JavaScript ..... 252
来源：http://3g.sjlbkw.cn/Article/details/gypqwzyge.sHtML

TypeScript ..... 212
来源：http://baike.fktsv.cn/Article/details/gyxreymqe.sHtML

Java ........... 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqepcdsz.sHtML

Go ............. 212
来源：http://www.blog.epnwcf.com/Article/details/gpoejbgob.sHtML

Ruby ........... 212
来源：http://mobile.tarul.cn/Article/details/gqqqqdyjx.sHtML

C# ............. 212
来源：http://mobile.vehdjk.com/Article/details/ggtaoafwx.sHtML

C .............. 30
来源：http://3g.fktsv.cn/Article/details/ggoskzfby.sHtML

C++ ............ 30
来源：http://3g.fktsv.cn/Article/details/gftkirxdp.sHtML

SQL ............ 90
来源：http://www.blog.vehdjk.com/Article/details/gucaupxkh.sHtML

Bash ........... 80
来源：http://blog.sjlbkw.cn/Article/details/gaerftdwi.sHtML

Kotlin ......... 15
来源：http://www.blog.sjlbkw.cn/Article/details/gmiuukpqp.sHtML

Swift .......... 15
来源：http://m.share.sjlbkw.cn/Article/details/guwxmuhzq.sHtML

Lua ............ 10
来源：http://baike.sjlbkw.cn/Article/details/ggzbsfepr.sHtML

Perl ........... 10
来源：http://mobile.yfazqb.com/Article/details/gikbokein.sHtML

Scala .......... 10
来源：http://read.share.yfazqb.com/Article/details/gykyzdmdd.sHtML

------------------------------------
来源：http://m.share.vehdjk.com/Article/details/gvlcvbtxn.sHtML

合计 ........... 2106 条
来源：http://m.share.vehdjk.com/Article/details/gelgmgfjb.sHtML

按章节统计：
来源：http://wap.fktsv.cn/Article/details/gxfqotvnk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fktsv.cn/Article/details/gdgkafwvm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.vehdjk.com/Article/details/gwjuliqns.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fktsv.cn/Article/details/grqdlknuf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.vehdjk.com/Article/details/gdfyjfequ.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.tarul.cn/Article/details/gueebkrbr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.vehdjk.com/Article/details/gxjmzdrjl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fktsv.cn/Article/details/grshwsfdl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.vehdjk.com/Article/details/gawwetaqn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.tarul.cn/Article/details/gtrvwhhoc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.yfazqb.com/Article/details/grcnmukql.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.yfazqb.com/Article/details/gtmcjcbwk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.vehdjk.com/Article/details/gkztpipus.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.yfazqb.com/Article/details/gnectdisu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.epnwcf.com/Article/details/gsylrpxys.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fktsv.cn/Article/details/ggyqrgbss.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/gziutfqds.sHtML

Q SQL 专题                              90
来源：http://www.m.share.vehdjk.com/Article/details/giemzunja.sHtML

R Bash 专题                             80
来源：http://www.share.tarul.cn/Article/details/gamwcswsu.sHtML

S C / C++ 专题                          60
来源：http://mobile.tarul.cn/Article/details/giqryolur.sHtML

T 其他语言补充                          60
来源：http://wap.bbcook.cn/Article/details/gxhanpria.sHtML

U 高频实用片段                         120
来源：http://www.share.tarul.cn/Article/details/gjotuzfgp.sHtML

------------------------------------
来源：http://3g.epnwcf.com/Article/details/gcxfazzgu.sHtML

合计                                  2106 条
来源：http://blog.vehdjk.com/Article/details/gltroflqq.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.sjlbkw.cn/Article/details/gxmdginvv.sHtML

使用提醒
来源：http://mobile.fktsv.cn/Article/details/gaijlztqi.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.vehdjk.com/Article/details/gusrhohsk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.vehdjk.com/Article/details/geyguvfjl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.bbcook.cn/Article/details/ghcmdslak.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fktsv.cn/Article/details/gmudndjec.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fktsv.cn/Article/details/gnvmsfilf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.bbcook.cn/Article/details/gprqqhwhd.sHtML

—— 文件结束 ——
来源：http://read.share.vehdjk.com/Article/details/gurwdvjnb.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gunafywhv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.bbcook.cn/Article/details/gjphdxoug.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.tarul.cn/Article/details/gclkwlfkg.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gdijbsepu.sHtML

【收录内容】
来源：http://wap.vehdjk.com/Article/details/ghsphvfyx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.yfazqb.com/Article/details/gcrbpdcvu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.vehdjk.com/Article/details/gtvdesklx.sHtML

SQL · Bash · C · C++
来源：http://www.blog.sjlbkw.cn/Article/details/gwhdiqkbd.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.bbcook.cn/Article/details/gtivulxee.sHtML

【使用说明】
来源：http://blog.bbcook.cn/Article/details/gkdvrdgmb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.yfazqb.com/Article/details/gmsmjfpuo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.sjlbkw.cn/Article/details/grjtdcptw.sHtML


<!-- 参考信息 -->