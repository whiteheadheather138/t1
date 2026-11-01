代发 wailian999

case class User(name: String, age: Int)
来源：http://baike.fktsv.cn/Article/details/goojalllr.sHtML

[T57] Scala：模式匹配
来源：http://blog.tarul.cn/Article/details/gchmihwnb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.sjlbkw.cn/Article/details/gfqjvezzu.sHtML

[T58] Scala：函数定义
来源：http://read.share.bbcook.cn/Article/details/gcoisarud.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.yfazqb.com/Article/details/gwrmgwbqk.sHtML

[T59] Scala：循环
来源：http://read.share.sjlbkw.cn/Article/details/gmwzglauc.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.epnwcf.com/Article/details/gfajfxmgx.sHtML

[T60] Scala：折叠
来源：http://3g.tarul.cn/Article/details/glfpmgfis.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.bbcook.cn/Article/details/guclwehjw.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gsneyftgl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.epnwcf.com/Article/details/gjypjvcyu.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gpprqwfej.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.sjlbkw.cn/Article/details/gkgbxvzta.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.tarul.cn/Article/details/gcslwbbfj.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.sjlbkw.cn/Article/details/gbnxstamk.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baike.fktsv.cn/Article/details/gqgshndlx.sHtML

[U03] Py：加载 .env 配置
来源：http://m.share.tarul.cn/Article/details/gqmahxdoi.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.yfazqb.com/Article/details/gpbmfpoaq.sHtML

[U04] Py：变量调试打印
来源：http://3g.sjlbkw.cn/Article/details/gjktgdnzq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.fktsv.cn/Article/details/gzucsdvif.sHtML

[U05] Py：列表去重且保序
来源：http://read.share.epnwcf.com/Article/details/gtvfiarej.sHtML

list(dict.fromkeys(arr))
来源：http://m.share.tarul.cn/Article/details/gxzhzcseb.sHtML

[U06] Py：合并两个字典
来源：http://www.share.fktsv.cn/Article/details/glhltifvn.sHtML

{**a, **b}
来源：http://mobile.fktsv.cn/Article/details/gezeimudz.sHtML

[U07] Py：反转字典键值
来源：http://baike.vehdjk.com/Article/details/goxltzkqo.sHtML

{v: k for k, v in d.items()}
来源：http://read.share.vehdjk.com/Article/details/gbdhccuwv.sHtML

[U08] Py：展平二维列表
来源：http://wap.vehdjk.com/Article/details/gezpvaknl.sHtML

[y for x in nested for y in x]
来源：http://www.share.sjlbkw.cn/Article/details/gcoitaqbv.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.tarul.cn/Article/details/gbfiendgh.sHtML

max(d, key=d.get)
来源：http://read.share.vehdjk.com/Article/details/gznalxhme.sHtML

[U10] Py：按值排序字典
来源：http://www.share.bbcook.cn/Article/details/gpexsuanu.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://blog.yfazqb.com/Article/details/glvubmknv.sHtML

[U11] Py：生成器表达式
来源：http://baike.tarul.cn/Article/details/grvjrjvfg.sHtML

(x * 2 for x in arr)
来源：http://blog.epnwcf.com/Article/details/gijwwcaky.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.share.sjlbkw.cn/Article/details/gphliofvk.sHtML

Counter(arr).most_common(3)
来源：http://3g.tarul.cn/Article/details/gvzvlzhgl.sHtML

[U13] Py：固定长度队列
来源：http://wap.epnwcf.com/Article/details/gkcwtqbjq.sHtML

deque(maxlen=10)
来源：http://read.share.fktsv.cn/Article/details/gmizirzcc.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.sjlbkw.cn/Article/details/gtuiogvwv.sHtML

defaultdict(list)
来源：http://mobile.tarul.cn/Article/details/gekwaumuo.sHtML

[U15] Py：高精度计时
来源：http://www.share.yfazqb.com/Article/details/gtsunzdov.sHtML

t = time.perf_counter()
来源：http://wap.tarul.cn/Article/details/gqibnvork.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fktsv.cn/Article/details/ggzwfjjsz.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.fktsv.cn/Article/details/gdyuwdmmm.sHtML

[U17] Py：初始化日志
来源：http://www.blog.epnwcf.com/Article/details/gjggdjfep.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.epnwcf.com/Article/details/gzecuyjhr.sHtML

[U18] Py：预编译正则
来源：http://3g.bbcook.cn/Article/details/ggqouprxd.sHtML

pat = re.compile(r"\d+")
来源：http://www.m.share.fktsv.cn/Article/details/gqmeijcuc.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.yfazqb.com/Article/details/gbymxoxfd.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.yfazqb.com/Article/details/gbfmrounb.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.epnwcf.com/Article/details/gxatblomg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.fktsv.cn/Article/details/gaigothew.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.tarul.cn/Article/details/gfmunbcxg.sHtML

@contextlib.contextmanager
来源：http://baike.sjlbkw.cn/Article/details/gzgrvkqcs.sHtML

[U22] Py：矩阵转置
来源：http://3g.bbcook.cn/Article/details/gyzofxmdt.sHtML

list(zip(*m))
来源：http://3g.vehdjk.com/Article/details/gnuxunkui.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.sjlbkw.cn/Article/details/gqgbanpwm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.bbcook.cn/Article/details/ggjlidsbl.sHtML

[U24] Py：路径操作
来源：http://read.share.yfazqb.com/Article/details/gkgshkdpr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.tarul.cn/Article/details/gaixvfizk.sHtML

[U25] Py：CSV 按字典读
来源：http://www.share.fktsv.cn/Article/details/gjiriphuy.sHtML

csv.DictReader(f)
来源：http://www.share.bbcook.cn/Article/details/ggrxgfgbb.sHtML

[U26] Py：并发下载
来源：http://blog.epnwcf.com/Article/details/gzihowdhr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.yfazqb.com/Article/details/gjscvprly.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.tarul.cn/Article/details/gknbydglj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.vehdjk.com/Article/details/guzceqkas.sHtML

[U28] Py：类型别名
来源：http://mobile.tarul.cn/Article/details/gqdtwuxdv.sHtML

UserId = int
来源：http://baike.yfazqb.com/Article/details/gwanovmas.sHtML

[U29] Py：属性校验
来源：http://wap.yfazqb.com/Article/details/gwevchvvg.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.yfazqb.com/Article/details/gpvgtbcrt.sHtML

[U30] Py：数据类
来源：http://wap.fktsv.cn/Article/details/gbrsewlvr.sHtML

@dataclass(slots=True)
来源：http://www.share.vehdjk.com/Article/details/gzvpmcxdr.sHtML

[U31] Py：单测
来源：http://www.blog.bbcook.cn/Article/details/gubkvgnjg.sHtML

python -m pytest -q
来源：http://blog.epnwcf.com/Article/details/gkavirnco.sHtML

[U32] Py：代码格式化
来源：http://www.share.sjlbkw.cn/Article/details/gzxxwjdpb.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.bbcook.cn/Article/details/gkrghzyly.sHtML

[U33] Py：打包发布
来源：http://blog.bbcook.cn/Article/details/gqhkzlxcn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.yfazqb.com/Article/details/gltbqgkhu.sHtML

[U34] Py：判断编码
来源：http://blog.bbcook.cn/Article/details/gagoxpnte.sHtML

chardet.detect(raw)
来源：http://www.share.fktsv.cn/Article/details/gvrhsmcqb.sHtML

[U35] Py：发送邮件
来源：http://www.share.vehdjk.com/Article/details/gjtvupehg.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.bbcook.cn/Article/details/gfbjyoyqn.sHtML

[U36] Py：定时任务
来源：http://www.share.sjlbkw.cn/Article/details/ghtdhcezy.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.fktsv.cn/Article/details/gdjemgqml.sHtML

[U37] Py：读写 Excel
来源：http://3g.tarul.cn/Article/details/gyuwtdvwo.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.yfazqb.com/Article/details/gaetvqzen.sHtML

[U38] Py：获取脚本所在目录
来源：http://read.share.yfazqb.com/Article/details/gnsqihbhg.sHtML

Path(__file__).resolve().parent
来源：http://wap.sjlbkw.cn/Article/details/gvamaejly.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.vehdjk.com/Article/details/gfyhczjuo.sHtML

sys.stdout.isatty()
来源：http://baike.sjlbkw.cn/Article/details/gskbtreso.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.epnwcf.com/Article/details/gckqqbkvl.sHtML

print("err", file=sys.stderr)
来源：http://3g.fktsv.cn/Article/details/gqubxrjlj.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.sjlbkw.cn/Article/details/gufwsvfte.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.sjlbkw.cn/Article/details/ghazxbgei.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.vehdjk.com/Article/details/ghrodzfud.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.yfazqb.com/Article/details/guulnsctl.sHtML

[U43] PHP：声明命名空间
来源：http://blog.epnwcf.com/Article/details/gqjjabcrn.sHtML

namespace App\Http;
来源：http://blog.epnwcf.com/Article/details/grdyoqjvd.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.epnwcf.com/Article/details/gxrcibhxx.sHtML

declare(strict_types=1);
来源：http://www.share.yfazqb.com/Article/details/gejqlyopo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.tarul.cn/Article/details/gxmgjwcfq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.yfazqb.com/Article/details/gbktkgtuv.sHtML

[U46] PHP：可空类型
来源：http://baike.fktsv.cn/Article/details/gukcpjlzg.sHtML

?string $name = null
来源：http://www.blog.epnwcf.com/Article/details/geglemnrs.sHtML

[U47] PHP：联合类型
来源：http://read.share.yfazqb.com/Article/details/gnplepqwa.sHtML

int|string $id
来源：http://wap.epnwcf.com/Article/details/guwsxoeqa.sHtML

[U48] PHP：纯枚举
来源：http://blog.epnwcf.com/Article/details/gknnzdvyd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.yfazqb.com/Article/details/gdqqchstq.sHtML

[U49] PHP：只读属性
来源：http://wap.vehdjk.com/Article/details/gkeqejlta.sHtML

public readonly string $name
来源：http://read.share.tarul.cn/Article/details/ghjyrftkj.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.tarul.cn/Article/details/gdzhtjsgr.sHtML

public function __construct(private int $id) {}
来源：http://www.blog.tarul.cn/Article/details/gvtqhxjjb.sHtML

[U51] PHP：数组解构
来源：http://read.share.epnwcf.com/Article/details/gdwnjeepu.sHtML

[$a, $b] = $arr;
来源：http://3g.yfazqb.com/Article/details/goxmvlqan.sHtML

[U52] PHP：箭头函数
来源：http://3g.yfazqb.com/Article/details/gnqpsyymp.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.tarul.cn/Article/details/gmsvfnjwm.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.bbcook.cn/Article/details/gpiapomtj.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.tarul.cn/Article/details/grmcuefgi.sHtML

[U54] PHP：空安全调用
来源：http://read.share.yfazqb.com/Article/details/getyhufbl.sHtML

$obj?->method()
来源：http://www.m.share.fktsv.cn/Article/details/grptzroai.sHtML

[U55] PHP：match 表达式
来源：http://wap.bbcook.cn/Article/details/gndgxxlhg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://baike.bbcook.cn/Article/details/gquoyfgrm.sHtML

[U56] PHP：命名参数
来源：http://read.share.vehdjk.com/Article/details/gwvolecbb.sHtML

f(a: 1, b: 2)
来源：http://mobile.vehdjk.com/Article/details/ggiztnddv.sHtML

[U57] PHP：字符串插值
来源：http://mobile.yfazqb.com/Article/details/gmwpgvndj.sHtML

"值: {$a}"
来源：http://mobile.yfazqb.com/Article/details/gomtnfisb.sHtML

[U58] PHP：数组三件套
来源：http://baike.fktsv.cn/Article/details/gavzacfqf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.tarul.cn/Article/details/gnwybwwfm.sHtML

[U59] PHP：自定义排序
来源：http://read.share.yfazqb.com/Article/details/gxjoslkat.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.bbcook.cn/Article/details/gwvkrhziq.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.vehdjk.com/Article/details/gmewmcxgw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.tarul.cn/Article/details/gxtjbycvi.sHtML

[U61] PHP：正则
来源：http://mobile.yfazqb.com/Article/details/gpiinnxce.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.bbcook.cn/Article/details/gqszpfses.sHtML

[U62] PHP：日期对象
来源：http://m.share.fktsv.cn/Article/details/gvmiykcxy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.sjlbkw.cn/Article/details/gbkvlugya.sHtML

[U63] PHP：文件读写
来源：http://mobile.bbcook.cn/Article/details/gxexxpuyf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.vehdjk.com/Article/details/ghblyrkth.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gyusczxds.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.yfazqb.com/Article/details/gdtongobs.sHtML

[U65] PHP：会话
来源：http://blog.vehdjk.com/Article/details/gikosbfml.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gondxduqd.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.vehdjk.com/Article/details/gyoodsent.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fktsv.cn/Article/details/gnyyqdtcc.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.yfazqb.com/Article/details/gufjvpwdu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.yfazqb.com/Article/details/gvvezmbxl.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.sjlbkw.cn/Article/details/geqwavvud.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.tarul.cn/Article/details/gjpllyvre.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.yfazqb.com/Article/details/gcjyhnsbe.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.epnwcf.com/Article/details/grmgdsolu.sHtML

[U70] PHP：PDO 事务
来源：http://3g.epnwcf.com/Article/details/gfwujhouq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.vehdjk.com/Article/details/gwjrsqtac.sHtML

[U71] PHP：抛出异常
来源：http://baike.fktsv.cn/Article/details/gyjugjudz.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.vehdjk.com/Article/details/gzdnucnxj.sHtML

[U72] PHP：写错误日志
来源：http://wap.tarul.cn/Article/details/gwtfnvspm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.bbcook.cn/Article/details/gxzxtrvjz.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.bbcook.cn/Article/details/gblwbkoir.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.epnwcf.com/Article/details/gdmkdpuqh.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.bbcook.cn/Article/details/gtxypqkzm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.epnwcf.com/Article/details/galelpvsv.sHtML

[U75] PHP：依赖注入
来源：http://wap.fktsv.cn/Article/details/gtaxlkikv.sHtML

composer require psr/container
来源：http://read.share.yfazqb.com/Article/details/ggoaytsof.sHtML

[U76] PHP：简单路由
来源：http://3g.epnwcf.com/Article/details/gkqtityoh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.fktsv.cn/Article/details/gqgwrvtqo.sHtML

[U77] PHP：模板渲染
来源：http://blog.yfazqb.com/Article/details/gmhnccdsm.sHtML

composer require twig/twig
来源：http://mobile.epnwcf.com/Article/details/grvttnagv.sHtML

[U78] PHP：单元测试
来源：http://blog.vehdjk.com/Article/details/gwioagpol.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.yfazqb.com/Article/details/gtulpxkos.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.yfazqb.com/Article/details/gwmnntcen.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.sjlbkw.cn/Article/details/gxmptwwjg.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fktsv.cn/Article/details/gumsrbbne.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.vehdjk.com/Article/details/gajwhnvbb.sHtML

[U81] JS：初始化项目
来源：http://blog.sjlbkw.cn/Article/details/gmveneqsy.sHtML

npm init -y;  npm i express
来源：http://www.m.share.epnwcf.com/Article/details/gyovtcudc.sHtML

[U82] JS：package.json 脚本
来源：http://wap.fktsv.cn/Article/details/gxbecviqy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.tarul.cn/Article/details/gokytnddr.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fktsv.cn/Article/details/glrbdsmtx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fktsv.cn/Article/details/gejxgzdqn.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.yfazqb.com/Article/details/gcugkjdcl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.yfazqb.com/Article/details/gxijuhxob.sHtML

[U85] JS：可选链
来源：http://m.share.epnwcf.com/Article/details/gsbzdhata.sHtML

a?.b?.c
来源：http://www.blog.epnwcf.com/Article/details/gspqrbsmy.sHtML

[U86] JS：空值合并
来源：http://blog.bbcook.cn/Article/details/gkbwfsdmq.sHtML

a ?? b
来源：http://blog.fktsv.cn/Article/details/gpznbpypi.sHtML

[U87] JS：解构默认值
来源：http://baike.epnwcf.com/Article/details/gdlfoxyhc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.sjlbkw.cn/Article/details/gflozzakz.sHtML

[U88] JS：对象展开合并
来源：http://blog.yfazqb.com/Article/details/gwjvxsjhx.sHtML

{ ...a, ...b }
来源：http://wap.tarul.cn/Article/details/gjxukhkyz.sHtML

[U89] JS：数组去重
来源：http://baike.fktsv.cn/Article/details/gploohldk.sHtML

[...new Set(arr)]
来源：http://3g.tarul.cn/Article/details/ggwyzgcag.sHtML

[U90] JS：数字数组排序
来源：http://3g.tarul.cn/Article/details/gzwyoeqgj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/ghrzupyhb.sHtML

[U91] JS：对象键值遍历
来源：http://3g.bbcook.cn/Article/details/girynqlmb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.bbcook.cn/Article/details/grkirwztf.sHtML

[U92] JS：深拷贝
来源：http://mobile.vehdjk.com/Article/details/gocefdqjp.sHtML

structuredClone(obj)
来源：http://read.share.tarul.cn/Article/details/gvaseqvxo.sHtML

[U93] JS：模板字符串
来源：http://baike.fktsv.cn/Article/details/gvcmsfels.sHtML

`共 ${n} 条`
来源：http://www.m.share.yfazqb.com/Article/details/gtztklsen.sHtML

[U94] JS：箭头函数
来源：http://m.share.vehdjk.com/Article/details/gfvtzrsxf.sHtML

const double = x => x * 2;
来源：http://3g.sjlbkw.cn/Article/details/giymncfnx.sHtML

[U95] JS：Promise 包装
来源：http://www.share.yfazqb.com/Article/details/gddowkcrd.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.bbcook.cn/Article/details/grbbgrnvj.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.sjlbkw.cn/Article/details/gjeqwfuwo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.yfazqb.com/Article/details/gkaugujbn.sHtML

[U97] JS：并发请求
来源：http://3g.sjlbkw.cn/Article/details/ghnjijyxq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fktsv.cn/Article/details/geifwihho.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.bbcook.cn/Article/details/gosxcaoxt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fktsv.cn/Article/details/gbximwbti.sHtML

[U99] JS：事件监听
来源：http://m.share.bbcook.cn/Article/details/gtfxpmbgs.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.sjlbkw.cn/Article/details/gmoisxrml.sHtML

[U100] JS：DOM 查询
来源：http://baike.fktsv.cn/Article/details/gkewltglj.sHtML

document.querySelector(".item")
来源：http://m.share.vehdjk.com/Article/details/gbkopvxql.sHtML

[U101] JS：classList 操作
来源：http://mobile.yfazqb.com/Article/details/gwzgpiowp.sHtML

el.classList.toggle("active")
来源：http://mobile.bbcook.cn/Article/details/gthcigcti.sHtML

[U102] JS：本地存储
来源：http://mobile.yfazqb.com/Article/details/gnmuoiopf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.bbcook.cn/Article/details/gyxpvklms.sHtML

[U103] JS：定时器
来源：http://www.share.tarul.cn/Article/details/gomrjsyzf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.tarul.cn/Article/details/glolyeirv.sHtML

[U104] JS：防抖
来源：http://mobile.epnwcf.com/Article/details/giegvyjqq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.sjlbkw.cn/Article/details/gmdfoxnwd.sHtML

[U105] JS：节流
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbesxxys.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.tarul.cn/Article/details/gzmgnfyvc.sHtML

[U106] JS：日期格式化
来源：http://wap.yfazqb.com/Article/details/gddfygnlb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.bbcook.cn/Article/details/gsmbaukam.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.bbcook.cn/Article/details/gkqadkbrd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.epnwcf.com/Article/details/gpvfequwh.sHtML

[U108] JS：随机整数
来源：http://baike.yfazqb.com/Article/details/gucmnakqx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.yfazqb.com/Article/details/giutoqyal.sHtML

[U109] JS：数组分组
来源：http://blog.epnwcf.com/Article/details/gvnnhvkxj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.yfazqb.com/Article/details/ghwjrljyi.sHtML

[U110] JS：数组分块
来源：http://blog.fktsv.cn/Article/details/gspvuekwb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.yfazqb.com/Article/details/glcsviovj.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fktsv.cn/Article/details/guxdiwvdb.sHtML

new Map(Object.entries(obj))
来源：http://mobile.tarul.cn/Article/details/ghzwzftnl.sHtML

[U112] JS：字符串补位
来源：http://3g.epnwcf.com/Article/details/ggdydtvmz.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/gncpykosn.sHtML

[U113] JS：正则替换全部
来源：http://mobile.yfazqb.com/Article/details/gctfqhmrx.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/gidcanxbv.sHtML

[U114] JS：JSON 深比较
来源：http://baike.vehdjk.com/Article/details/gfmsflphm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fktsv.cn/Article/details/gvdqlrfxo.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fktsv.cn/Article/details/gblykkicq.sHtML

crypto.randomUUID()
来源：http://www.blog.vehdjk.com/Article/details/guehmcrak.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.vehdjk.com/Article/details/gxqxibuhh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.sjlbkw.cn/Article/details/giwvnxtss.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fktsv.cn/Article/details/gdurkhxgg.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.sjlbkw.cn/Article/details/gorxpgsuf.sHtML

[U118] JS：开发服务器
来源：http://m.share.yfazqb.com/Article/details/gboytayua.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.tarul.cn/Article/details/gowpcghqq.sHtML

[U119] JS：生产构建
来源：http://www.blog.vehdjk.com/Article/details/gulvkbjyk.sHtML

npx vite build
来源：http://www.share.bbcook.cn/Article/details/gtqjtwabv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.epnwcf.com/Article/details/gyrfamhyh.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.yfazqb.com/Article/details/grzzaawcg.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gzkbdkkmv.sHtML

统计汇总
来源：http://www.m.share.yfazqb.com/Article/details/gldakgxnw.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gajjcfroe.sHtML

按语言统计（条）：
来源：http://3g.yfazqb.com/Article/details/gyljuvcls.sHtML

Python ......... 252
来源：http://www.blog.bbcook.cn/Article/details/gaocwxggo.sHtML

PHP ............ 252
来源：http://www.m.share.vehdjk.com/Article/details/gcisreksw.sHtML

JavaScript ..... 252
来源：http://mobile.tarul.cn/Article/details/gpxixnkcf.sHtML

TypeScript ..... 212
来源：http://www.blog.fktsv.cn/Article/details/gmdstszmo.sHtML

Java ........... 212
来源：http://www.m.share.fktsv.cn/Article/details/gxlyoeetu.sHtML

Go ............. 212
来源：http://www.share.tarul.cn/Article/details/gjonnvjbu.sHtML

Ruby ........... 212
来源：http://read.share.vehdjk.com/Article/details/gpuxlhyxk.sHtML

C# ............. 212
来源：http://www.share.yfazqb.com/Article/details/gooxooziv.sHtML

C .............. 30
来源：http://blog.yfazqb.com/Article/details/gegwhnebn.sHtML

C++ ............ 30
来源：http://www.share.vehdjk.com/Article/details/gzhaitvnp.sHtML

SQL ............ 90
来源：http://mobile.bbcook.cn/Article/details/gzzzjeela.sHtML

Bash ........... 80
来源：http://mobile.vehdjk.com/Article/details/gcgrynung.sHtML

Kotlin ......... 15
来源：http://www.blog.yfazqb.com/Article/details/ghtpjnltc.sHtML

Swift .......... 15
来源：http://m.share.epnwcf.com/Article/details/ghvqvfddq.sHtML

Lua ............ 10
来源：http://www.m.share.yfazqb.com/Article/details/gbmxthggg.sHtML

Perl ........... 10
来源：http://3g.bbcook.cn/Article/details/gladcjxqr.sHtML

Scala .......... 10
来源：http://www.blog.vehdjk.com/Article/details/gmhbaewiz.sHtML

------------------------------------
来源：http://blog.tarul.cn/Article/details/gfticofut.sHtML

合计 ........... 2106 条
来源：http://wap.sjlbkw.cn/Article/details/glmfhatum.sHtML

按章节统计：
来源：http://www.blog.epnwcf.com/Article/details/gpluglaxh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.yfazqb.com/Article/details/gkntntmlc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.tarul.cn/Article/details/gkoofpezs.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.bbcook.cn/Article/details/gknjfctus.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.epnwcf.com/Article/details/gurydayuc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.tarul.cn/Article/details/gtavbltlu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.tarul.cn/Article/details/gdjvajnum.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.sjlbkw.cn/Article/details/gufjkoosw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.tarul.cn/Article/details/gnfewqdqq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.sjlbkw.cn/Article/details/gevuetcml.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.yfazqb.com/Article/details/gvnqihfim.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gljvlzcdy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/gvrpkdrxd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/gvfludmjc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.sjlbkw.cn/Article/details/gcbkrrzya.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.yfazqb.com/Article/details/guvzrtfig.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/guaxhywrl.sHtML

Q SQL 专题                              90
来源：http://blog.vehdjk.com/Article/details/gdaukspvx.sHtML

R Bash 专题                             80
来源：http://3g.yfazqb.com/Article/details/gczjpjwfv.sHtML

S C / C++ 专题                          60
来源：http://www.blog.epnwcf.com/Article/details/gugnulxgs.sHtML

T 其他语言补充                          60
来源：http://blog.yfazqb.com/Article/details/guxqwbeuc.sHtML

U 高频实用片段                         120
来源：http://wap.bbcook.cn/Article/details/gxvvovrui.sHtML

------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/gahdfisby.sHtML

合计                                  2106 条
来源：http://www.blog.yfazqb.com/Article/details/gmrjqcigs.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fktsv.cn/Article/details/gmglxorab.sHtML


<!-- 参考信息 -->