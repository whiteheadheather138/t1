代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://wap.bbcook.cn/Article/details/gidslvfft.sHtML

[T55] Scala：集合过滤
来源：http://blog.sjlbkw.cn/Article/details/glhjhvsbj.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fktsv.cn/Article/details/gdmjxaowy.sHtML

[T56] Scala：样例类
来源：http://wap.yfazqb.com/Article/details/gmdspaqij.sHtML

case class User(name: String, age: Int)
来源：http://read.share.vehdjk.com/Article/details/gdxhbiego.sHtML

[T57] Scala：模式匹配
来源：http://wap.sjlbkw.cn/Article/details/ghjpzewbg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fktsv.cn/Article/details/glftqnjjr.sHtML

[T58] Scala：函数定义
来源：http://baike.epnwcf.com/Article/details/gbhurudlh.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.tarul.cn/Article/details/gqzdfkmsq.sHtML

[T59] Scala：循环
来源：http://www.m.share.tarul.cn/Article/details/gswwjyuih.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fktsv.cn/Article/details/gzxjiherb.sHtML

[T60] Scala：折叠
来源：http://baike.bbcook.cn/Article/details/glzwdgpvv.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.sjlbkw.cn/Article/details/giajwrivd.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gqktjupig.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.yfazqb.com/Article/details/gbvxtvlhr.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gbyamvgdp.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.yfazqb.com/Article/details/gssmpjbda.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://3g.bbcook.cn/Article/details/ghemfmygw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.vehdjk.com/Article/details/gignrxkhh.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.vehdjk.com/Article/details/gebzeiois.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.fktsv.cn/Article/details/gydeyfrrn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.sjlbkw.cn/Article/details/gfujsgrxx.sHtML

[U04] Py：变量调试打印
来源：http://m.share.tarul.cn/Article/details/ghixgohad.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.blog.fktsv.cn/Article/details/gwjnrehow.sHtML

[U05] Py：列表去重且保序
来源：http://baike.vehdjk.com/Article/details/gyascamzc.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.tarul.cn/Article/details/gvbfgmvjy.sHtML

[U06] Py：合并两个字典
来源：http://blog.yfazqb.com/Article/details/grcuuwntd.sHtML

{**a, **b}
来源：http://mobile.epnwcf.com/Article/details/gitpplmsx.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.vehdjk.com/Article/details/gjgjinohw.sHtML

{v: k for k, v in d.items()}
来源：http://wap.bbcook.cn/Article/details/guyazkbrz.sHtML

[U08] Py：展平二维列表
来源：http://mobile.yfazqb.com/Article/details/gssdnuywt.sHtML

[y for x in nested for y in x]
来源：http://read.share.tarul.cn/Article/details/gaiuhgbje.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.fktsv.cn/Article/details/giffzwbxo.sHtML

max(d, key=d.get)
来源：http://www.m.share.tarul.cn/Article/details/glpaayhvj.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.tarul.cn/Article/details/glxurjrpn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.bbcook.cn/Article/details/gmtpgfgvv.sHtML

[U11] Py：生成器表达式
来源：http://m.share.epnwcf.com/Article/details/glpfhzcau.sHtML

(x * 2 for x in arr)
来源：http://3g.fktsv.cn/Article/details/guxanmyui.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.fktsv.cn/Article/details/gsaiwwluz.sHtML

Counter(arr).most_common(3)
来源：http://read.share.epnwcf.com/Article/details/gxfxncfiu.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.tarul.cn/Article/details/gfdssieqi.sHtML

deque(maxlen=10)
来源：http://baike.tarul.cn/Article/details/gyhsqccwc.sHtML

[U14] Py：分组收集到列表
来源：http://m.share.vehdjk.com/Article/details/gtcfxyfaf.sHtML

defaultdict(list)
来源：http://baike.tarul.cn/Article/details/gwhfsrsyv.sHtML

[U15] Py：高精度计时
来源：http://mobile.tarul.cn/Article/details/gkwospesm.sHtML

t = time.perf_counter()
来源：http://m.share.bbcook.cn/Article/details/gultidzuf.sHtML

[U16] Py：命令行参数解析
来源：http://baike.fktsv.cn/Article/details/gnrtoazgh.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.epnwcf.com/Article/details/gofhlwowf.sHtML

[U17] Py：初始化日志
来源：http://3g.fktsv.cn/Article/details/grvolltxw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwybqkjdr.sHtML

[U18] Py：预编译正则
来源：http://read.share.bbcook.cn/Article/details/gpxgfsoer.sHtML

pat = re.compile(r"\d+")
来源：http://3g.tarul.cn/Article/details/ghyhoxeuv.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.bbcook.cn/Article/details/gwpfjrgif.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.tarul.cn/Article/details/gphaolhrn.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.yfazqb.com/Article/details/gyamzvpxe.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.fktsv.cn/Article/details/gummpptuu.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.vehdjk.com/Article/details/gorlfzyqs.sHtML

@contextlib.contextmanager
来源：http://www.share.tarul.cn/Article/details/gkzqnwtvw.sHtML

[U22] Py：矩阵转置
来源：http://blog.sjlbkw.cn/Article/details/ghhwpqzot.sHtML

list(zip(*m))
来源：http://www.share.bbcook.cn/Article/details/ghwguxzlk.sHtML

[U23] Py：分块读取大文件
来源：http://3g.sjlbkw.cn/Article/details/gdbclvgrn.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.vehdjk.com/Article/details/gbodsnaxj.sHtML

[U24] Py：路径操作
来源：http://m.share.vehdjk.com/Article/details/guylsisyt.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.epnwcf.com/Article/details/gifoyluas.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.yfazqb.com/Article/details/gknppzxcq.sHtML

csv.DictReader(f)
来源：http://blog.sjlbkw.cn/Article/details/gwzmqblaa.sHtML

[U26] Py：并发下载
来源：http://read.share.tarul.cn/Article/details/gluvkybzf.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.sjlbkw.cn/Article/details/guwononbj.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.vehdjk.com/Article/details/gimwrodsp.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.bbcook.cn/Article/details/gdagtoteh.sHtML

[U28] Py：类型别名
来源：http://blog.epnwcf.com/Article/details/gsrobztfh.sHtML

UserId = int
来源：http://read.share.vehdjk.com/Article/details/ggdtpdxys.sHtML

[U29] Py：属性校验
来源：http://3g.tarul.cn/Article/details/gypkrvlfi.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.sjlbkw.cn/Article/details/gfqxizjrp.sHtML

[U30] Py：数据类
来源：http://read.share.sjlbkw.cn/Article/details/glowizpib.sHtML

@dataclass(slots=True)
来源：http://baike.bbcook.cn/Article/details/geqfufaxr.sHtML

[U31] Py：单测
来源：http://3g.sjlbkw.cn/Article/details/gtnmugvcg.sHtML

python -m pytest -q
来源：http://read.share.bbcook.cn/Article/details/gcgcfqxfo.sHtML

[U32] Py：代码格式化
来源：http://www.m.share.epnwcf.com/Article/details/gatvdlpcs.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.tarul.cn/Article/details/gvmcamlhq.sHtML

[U33] Py：打包发布
来源：http://www.m.share.bbcook.cn/Article/details/gxvvmzdfa.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://baike.fktsv.cn/Article/details/gybuxoclh.sHtML

[U34] Py：判断编码
来源：http://baike.vehdjk.com/Article/details/gjdrpgwdk.sHtML

chardet.detect(raw)
来源：http://www.m.share.bbcook.cn/Article/details/gyzwaxudf.sHtML

[U35] Py：发送邮件
来源：http://3g.vehdjk.com/Article/details/gbtvyckbe.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.vehdjk.com/Article/details/gwmjkpdix.sHtML

[U36] Py：定时任务
来源：http://www.blog.vehdjk.com/Article/details/gpuzhjdpb.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.yfazqb.com/Article/details/gnpleufii.sHtML

[U37] Py：读写 Excel
来源：http://m.share.yfazqb.com/Article/details/gsytssnbt.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.vehdjk.com/Article/details/geapadnma.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.yfazqb.com/Article/details/gqhvrdyjy.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.bbcook.cn/Article/details/gefydejbq.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.tarul.cn/Article/details/gvepfxhci.sHtML

sys.stdout.isatty()
来源：http://www.m.share.vehdjk.com/Article/details/gktwycpmh.sHtML

[U40] Py：打印到标准错误
来源：http://blog.tarul.cn/Article/details/ghtznjymb.sHtML

print("err", file=sys.stderr)
来源：http://read.share.epnwcf.com/Article/details/guyhzzygt.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://read.share.tarul.cn/Article/details/gwgsdalst.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://wap.tarul.cn/Article/details/gvqrdixnm.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.sjlbkw.cn/Article/details/ggtcosjkg.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.fktsv.cn/Article/details/gdwrmxzxb.sHtML

[U43] PHP：声明命名空间
来源：http://wap.sjlbkw.cn/Article/details/gjgadlchd.sHtML

namespace App\Http;
来源：http://3g.tarul.cn/Article/details/gqbhgqfso.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.vehdjk.com/Article/details/gknqvcakn.sHtML

declare(strict_types=1);
来源：http://www.share.tarul.cn/Article/details/gqjwjillo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.bbcook.cn/Article/details/gquwznypi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/gijpeidzq.sHtML

[U46] PHP：可空类型
来源：http://m.share.tarul.cn/Article/details/gbpnmdlah.sHtML

?string $name = null
来源：http://www.m.share.sjlbkw.cn/Article/details/guwselnhr.sHtML

[U47] PHP：联合类型
来源：http://read.share.vehdjk.com/Article/details/gvanesbuh.sHtML

int|string $id
来源：http://blog.tarul.cn/Article/details/gjeiwztdp.sHtML

[U48] PHP：纯枚举
来源：http://www.share.tarul.cn/Article/details/gmlvyujsr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.bbcook.cn/Article/details/gnkcpddzh.sHtML

[U49] PHP：只读属性
来源：http://www.blog.vehdjk.com/Article/details/ggyjmqium.sHtML

public readonly string $name
来源：http://read.share.tarul.cn/Article/details/gfzxpfpck.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.vehdjk.com/Article/details/gfinuctme.sHtML

public function __construct(private int $id) {}
来源：http://www.share.fktsv.cn/Article/details/gpegijmno.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.vehdjk.com/Article/details/gjsavcifq.sHtML

[$a, $b] = $arr;
来源：http://www.blog.bbcook.cn/Article/details/gsdpiuuth.sHtML

[U52] PHP：箭头函数
来源：http://m.share.epnwcf.com/Article/details/gazoafprz.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.bbcook.cn/Article/details/gsydnnsss.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.sjlbkw.cn/Article/details/gqnexxrpn.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fktsv.cn/Article/details/glfyflqcq.sHtML

[U54] PHP：空安全调用
来源：http://mobile.epnwcf.com/Article/details/gcpgyedyx.sHtML

$obj?->method()
来源：http://www.m.share.tarul.cn/Article/details/ghxgripui.sHtML

[U55] PHP：match 表达式
来源：http://mobile.yfazqb.com/Article/details/gmgoeniro.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.yfazqb.com/Article/details/gpstocbsp.sHtML

[U56] PHP：命名参数
来源：http://www.share.yfazqb.com/Article/details/grhqbjfbn.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fktsv.cn/Article/details/gvbdzqabz.sHtML

[U57] PHP：字符串插值
来源：http://baike.fktsv.cn/Article/details/guawfcuyb.sHtML

"值: {$a}"
来源：http://m.share.epnwcf.com/Article/details/gzqddmbvn.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.bbcook.cn/Article/details/geviqanzg.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gteyymdnx.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.bbcook.cn/Article/details/gehuwepld.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fktsv.cn/Article/details/gmqubkdby.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.sjlbkw.cn/Article/details/gqwkebzrw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fktsv.cn/Article/details/golkrhzww.sHtML

[U61] PHP：正则
来源：http://mobile.yfazqb.com/Article/details/grhlgttey.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.yfazqb.com/Article/details/grqsvjbbt.sHtML

[U62] PHP：日期对象
来源：http://read.share.yfazqb.com/Article/details/givwuovmd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fktsv.cn/Article/details/ggbnyroqy.sHtML

[U63] PHP：文件读写
来源：http://www.share.epnwcf.com/Article/details/gytpecmtl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.tarul.cn/Article/details/gudpzxtyz.sHtML

[U64] PHP：目录遍历
来源：http://m.share.bbcook.cn/Article/details/gsutvhupo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.bbcook.cn/Article/details/geonvcbmk.sHtML

[U65] PHP：会话
来源：http://www.m.share.sjlbkw.cn/Article/details/gpduzafes.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/gjuayscvx.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.fktsv.cn/Article/details/griulfsfa.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.bbcook.cn/Article/details/gigmfhfme.sHtML

[U67] PHP：处理文件上传
来源：http://blog.tarul.cn/Article/details/grwetvvur.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.vehdjk.com/Article/details/gttxauxdf.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.vehdjk.com/Article/details/gterayzhm.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.bbcook.cn/Article/details/gjgcirhna.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.yfazqb.com/Article/details/gmuveaxcd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.epnwcf.com/Article/details/gicdnlapo.sHtML

[U70] PHP：PDO 事务
来源：http://blog.bbcook.cn/Article/details/gddjbnocw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.bbcook.cn/Article/details/gukgssyfu.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.tarul.cn/Article/details/gngcsfyae.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.bbcook.cn/Article/details/golastbnv.sHtML

[U72] PHP：写错误日志
来源：http://baike.yfazqb.com/Article/details/gknizvxku.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.yfazqb.com/Article/details/getovvaho.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.epnwcf.com/Article/details/gjzqsgmfj.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpfkdyvb.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.bbcook.cn/Article/details/gcbkhesfg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.bbcook.cn/Article/details/gjnmddwoj.sHtML

[U75] PHP：依赖注入
来源：http://www.share.tarul.cn/Article/details/grbkwivgh.sHtML

composer require psr/container
来源：http://baike.sjlbkw.cn/Article/details/gnurwrqqh.sHtML

[U76] PHP：简单路由
来源：http://baike.fktsv.cn/Article/details/gyovbvjec.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fktsv.cn/Article/details/gkvisroxk.sHtML

[U77] PHP：模板渲染
来源：http://3g.bbcook.cn/Article/details/guwyedbww.sHtML

composer require twig/twig
来源：http://baike.sjlbkw.cn/Article/details/gypjfrxgr.sHtML

[U78] PHP：单元测试
来源：http://www.share.fktsv.cn/Article/details/gabdjsjmd.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.epnwcf.com/Article/details/grgplcltu.sHtML

[U79] PHP：静态分析
来源：http://3g.yfazqb.com/Article/details/gmmjfdrlw.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.tarul.cn/Article/details/gmlcfkghh.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.vehdjk.com/Article/details/gktzndbpa.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.tarul.cn/Article/details/gewngkfzr.sHtML

[U81] JS：初始化项目
来源：http://read.share.fktsv.cn/Article/details/ghywtpetj.sHtML

npm init -y;  npm i express
来源：http://blog.sjlbkw.cn/Article/details/gumgerken.sHtML

[U82] JS：package.json 脚本
来源：http://baike.bbcook.cn/Article/details/gnxcjdfty.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fktsv.cn/Article/details/gnucaqize.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fktsv.cn/Article/details/ggvmwzeaw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.epnwcf.com/Article/details/gshgdhxai.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.vehdjk.com/Article/details/grllpveer.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.yfazqb.com/Article/details/gelugtfoh.sHtML

[U85] JS：可选链
来源：http://baike.yfazqb.com/Article/details/gsppikqqw.sHtML

a?.b?.c
来源：http://wap.vehdjk.com/Article/details/gfridlfmo.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fktsv.cn/Article/details/gupeismgx.sHtML

a ?? b
来源：http://blog.yfazqb.com/Article/details/glaykdfhp.sHtML

[U87] JS：解构默认值
来源：http://m.share.epnwcf.com/Article/details/gnypcvxiu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.tarul.cn/Article/details/gckrfyryx.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.yfazqb.com/Article/details/gffztjzgn.sHtML

{ ...a, ...b }
来源：http://wap.bbcook.cn/Article/details/geefybyzo.sHtML

[U89] JS：数组去重
来源：http://baike.epnwcf.com/Article/details/gsngdvupm.sHtML

[...new Set(arr)]
来源：http://3g.vehdjk.com/Article/details/gekbfqqgd.sHtML

[U90] JS：数字数组排序
来源：http://m.share.bbcook.cn/Article/details/gbftumawh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gwlubghih.sHtML

[U91] JS：对象键值遍历
来源：http://wap.tarul.cn/Article/details/gplhiujib.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.vehdjk.com/Article/details/gjpddagzy.sHtML

[U92] JS：深拷贝
来源：http://www.share.epnwcf.com/Article/details/gitqnddpw.sHtML

structuredClone(obj)
来源：http://wap.sjlbkw.cn/Article/details/gizaocfqg.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/geqzqqvva.sHtML

`共 ${n} 条`
来源：http://www.m.share.bbcook.cn/Article/details/gnpajvgej.sHtML

[U94] JS：箭头函数
来源：http://m.share.yfazqb.com/Article/details/guxanybwq.sHtML

const double = x => x * 2;
来源：http://read.share.sjlbkw.cn/Article/details/gefahpbyg.sHtML

[U95] JS：Promise 包装
来源：http://3g.yfazqb.com/Article/details/gnhersjut.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.tarul.cn/Article/details/gvwyzmbql.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.yfazqb.com/Article/details/gxsyrtoah.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fktsv.cn/Article/details/gnhoreiss.sHtML

[U97] JS：并发请求
来源：http://read.share.yfazqb.com/Article/details/gozkpmknh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fktsv.cn/Article/details/gxpbijryq.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.yfazqb.com/Article/details/gqdtppkye.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.bbcook.cn/Article/details/ghifiygpj.sHtML

[U99] JS：事件监听
来源：http://www.m.share.epnwcf.com/Article/details/gpzlsolcd.sHtML

el.addEventListener("click", e => {})
来源：http://blog.tarul.cn/Article/details/gvhawnsfz.sHtML

[U100] JS：DOM 查询
来源：http://mobile.epnwcf.com/Article/details/gunxluclw.sHtML

document.querySelector(".item")
来源：http://baike.yfazqb.com/Article/details/gmjpjnntx.sHtML

[U101] JS：classList 操作
来源：http://mobile.tarul.cn/Article/details/gfjgrllsk.sHtML

el.classList.toggle("active")
来源：http://baike.bbcook.cn/Article/details/giohtsvfp.sHtML

[U102] JS：本地存储
来源：http://wap.vehdjk.com/Article/details/grfzjrkkf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.tarul.cn/Article/details/gepmrkawc.sHtML

[U103] JS：定时器
来源：http://blog.epnwcf.com/Article/details/grrriamcv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.bbcook.cn/Article/details/grdhovxep.sHtML

[U104] JS：防抖
来源：http://blog.sjlbkw.cn/Article/details/grqutmiau.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.tarul.cn/Article/details/gwyzumlaa.sHtML

[U105] JS：节流
来源：http://www.blog.yfazqb.com/Article/details/giarfluil.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.vehdjk.com/Article/details/ggpfoeobo.sHtML

[U106] JS：日期格式化
来源：http://3g.tarul.cn/Article/details/gzzlusybm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.yfazqb.com/Article/details/gyxnuyjhx.sHtML

[U107] JS：数字千分位
来源：http://wap.fktsv.cn/Article/details/gtcxyhujy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.epnwcf.com/Article/details/gpyksphmt.sHtML

[U108] JS：随机整数
来源：http://3g.fktsv.cn/Article/details/gyqscmqlr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.bbcook.cn/Article/details/gilxddnlq.sHtML

[U109] JS：数组分组
来源：http://3g.fktsv.cn/Article/details/giqpptnck.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.yfazqb.com/Article/details/gftlbojvr.sHtML

[U110] JS：数组分块
来源：http://www.blog.vehdjk.com/Article/details/gajmkevrn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fktsv.cn/Article/details/gxatvsdpz.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.bbcook.cn/Article/details/gdfcgvvab.sHtML

new Map(Object.entries(obj))
来源：http://www.share.yfazqb.com/Article/details/germpjdzt.sHtML

[U112] JS：字符串补位
来源：http://blog.fktsv.cn/Article/details/gzhgutzoo.sHtML

"7".padStart(3, "0")
来源：http://m.share.epnwcf.com/Article/details/gjalxrpnx.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.yfazqb.com/Article/details/gsszmgaca.sHtML

s.replaceAll("a", "b")
来源：http://read.share.sjlbkw.cn/Article/details/gwlplkzds.sHtML

[U114] JS：JSON 深比较
来源：http://baike.epnwcf.com/Article/details/gbtfmqacm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.bbcook.cn/Article/details/gfkhptfxf.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fktsv.cn/Article/details/giqjlckes.sHtML

crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/gwjyjlhzo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.bbcook.cn/Article/details/ghvqwwlgu.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.epnwcf.com/Article/details/gphbwlvly.sHtML

[U117] JS：单元测试
来源：http://baike.tarul.cn/Article/details/gotdnenjg.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fktsv.cn/Article/details/giupedlhg.sHtML

[U118] JS：开发服务器
来源：http://read.share.fktsv.cn/Article/details/gycapsoel.sHtML

npm i -D vite;  npx vite
来源：http://www.share.vehdjk.com/Article/details/gpmikfloz.sHtML

[U119] JS：生产构建
来源：http://read.share.vehdjk.com/Article/details/gidappscl.sHtML

npx vite build
来源：http://wap.epnwcf.com/Article/details/gjxbepoto.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.vehdjk.com/Article/details/gaffttoec.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fktsv.cn/Article/details/gvwwbjowa.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gbrcyfytx.sHtML

统计汇总
来源：http://www.blog.vehdjk.com/Article/details/gshkzikus.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gcttddycn.sHtML

按语言统计（条）：
来源：http://mobile.yfazqb.com/Article/details/gexgjidmd.sHtML

Python ......... 252
来源：http://m.share.bbcook.cn/Article/details/gdmqgezxh.sHtML

PHP ............ 252
来源：http://blog.epnwcf.com/Article/details/gisqajpcx.sHtML

JavaScript ..... 252
来源：http://mobile.yfazqb.com/Article/details/grxpejhed.sHtML

TypeScript ..... 212
来源：http://baike.vehdjk.com/Article/details/gsqxlottq.sHtML

Java ........... 212
来源：http://blog.vehdjk.com/Article/details/gwtaxwpef.sHtML

Go ............. 212
来源：http://blog.vehdjk.com/Article/details/ganupyfwh.sHtML

Ruby ........... 212
来源：http://m.share.vehdjk.com/Article/details/gaqcvinxs.sHtML

C# ............. 212
来源：http://www.share.vehdjk.com/Article/details/grmikhqvs.sHtML

C .............. 30
来源：http://3g.yfazqb.com/Article/details/gxuhulgul.sHtML

C++ ............ 30
来源：http://3g.tarul.cn/Article/details/gpqlmzssi.sHtML

SQL ............ 90
来源：http://blog.epnwcf.com/Article/details/gcgkbpduu.sHtML

Bash ........... 80
来源：http://m.share.epnwcf.com/Article/details/guyiipebo.sHtML

Kotlin ......... 15
来源：http://read.share.sjlbkw.cn/Article/details/gzdqjbddi.sHtML

Swift .......... 15
来源：http://m.share.yfazqb.com/Article/details/ggvvuqxed.sHtML

Lua ............ 10
来源：http://read.share.tarul.cn/Article/details/gitiivuyq.sHtML

Perl ........... 10
来源：http://baike.tarul.cn/Article/details/glvddwjxj.sHtML

Scala .......... 10
来源：http://www.m.share.bbcook.cn/Article/details/gtonptweg.sHtML

------------------------------------
来源：http://wap.yfazqb.com/Article/details/geqsbsfrr.sHtML

合计 ........... 2106 条
来源：http://blog.yfazqb.com/Article/details/guhkknkgq.sHtML

按章节统计：
来源：http://read.share.sjlbkw.cn/Article/details/gqmtuinhc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fktsv.cn/Article/details/gyvizjphq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fktsv.cn/Article/details/gksewedts.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.tarul.cn/Article/details/gecnkyuvq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.bbcook.cn/Article/details/gubtodiet.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.vehdjk.com/Article/details/gjhijvdqs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.tarul.cn/Article/details/gsibpidxa.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fktsv.cn/Article/details/gmgnnuoye.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.epnwcf.com/Article/details/gqzjqmzxa.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.vehdjk.com/Article/details/gwndsopkz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.epnwcf.com/Article/details/guzdpcpcd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.vehdjk.com/Article/details/gpylyklff.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.sjlbkw.cn/Article/details/gcsmpjfcg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.bbcook.cn/Article/details/gqifuhkyk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.yfazqb.com/Article/details/gmqmakjji.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.yfazqb.com/Article/details/gklxeiyes.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.yfazqb.com/Article/details/gxjzaneqs.sHtML

Q SQL 专题                              90
来源：http://www.m.share.yfazqb.com/Article/details/gyudoqgop.sHtML

R Bash 专题                             80
来源：http://m.share.sjlbkw.cn/Article/details/grbvgfcwy.sHtML

S C / C++ 专题                          60
来源：http://mobile.epnwcf.com/Article/details/gjnysfcil.sHtML

T 其他语言补充                          60
来源：http://wap.fktsv.cn/Article/details/gczzmtoey.sHtML


<!-- 参考信息 -->