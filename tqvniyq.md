代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://m.share.tarul.cn/Article/details/gsdgzehvt.sHtML

[T55] Scala：集合过滤
来源：http://3g.fktsv.cn/Article/details/gcumgkdkk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.epnwcf.com/Article/details/gonxxzjbt.sHtML

[T56] Scala：样例类
来源：http://www.share.yfazqb.com/Article/details/gjrrigdei.sHtML

case class User(name: String, age: Int)
来源：http://www.blog.tarul.cn/Article/details/glusqkjfk.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fktsv.cn/Article/details/gkjarpdcc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.sjlbkw.cn/Article/details/gaggadhlt.sHtML

[T58] Scala：函数定义
来源：http://wap.epnwcf.com/Article/details/gmycbusar.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fktsv.cn/Article/details/gupooiwxo.sHtML

[T59] Scala：循环
来源：http://m.share.tarul.cn/Article/details/gltcvqbjd.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.epnwcf.com/Article/details/gusiyrqhq.sHtML

[T60] Scala：折叠
来源：http://blog.yfazqb.com/Article/details/goltmypuf.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.fktsv.cn/Article/details/gxznxpxfi.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gtvlgtokf.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gzwaclgem.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gegqrxjud.sHtML

[U01] Py：创建虚拟环境
来源：http://baike.epnwcf.com/Article/details/gmgmfqkbf.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.share.vehdjk.com/Article/details/ggmlvoeah.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.yfazqb.com/Article/details/giktmpijv.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fktsv.cn/Article/details/gidfthieg.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.sjlbkw.cn/Article/details/gqbinrgsy.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.share.yfazqb.com/Article/details/gyufrijcs.sHtML

[U04] Py：变量调试打印
来源：http://read.share.sjlbkw.cn/Article/details/ghdkguvfz.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://3g.vehdjk.com/Article/details/gmqijmttw.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.tarul.cn/Article/details/gfkivhrng.sHtML

list(dict.fromkeys(arr))
来源：http://3g.fktsv.cn/Article/details/gqdpuokme.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.bbcook.cn/Article/details/gzadezerg.sHtML

{**a, **b}
来源：http://www.blog.sjlbkw.cn/Article/details/gugjwwpvi.sHtML

[U07] Py：反转字典键值
来源：http://blog.bbcook.cn/Article/details/gjgygoyox.sHtML

{v: k for k, v in d.items()}
来源：http://3g.fktsv.cn/Article/details/gnotzsfdp.sHtML

[U08] Py：展平二维列表
来源：http://baike.sjlbkw.cn/Article/details/gawiilnwt.sHtML

[y for x in nested for y in x]
来源：http://m.share.bbcook.cn/Article/details/geljpzbcf.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.tarul.cn/Article/details/gjtpfayud.sHtML

max(d, key=d.get)
来源：http://read.share.sjlbkw.cn/Article/details/gyhdfkeuk.sHtML

[U10] Py：按值排序字典
来源：http://wap.sjlbkw.cn/Article/details/gwlgaqexk.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.vehdjk.com/Article/details/gosjshdwz.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.bbcook.cn/Article/details/gzvznpdzd.sHtML

(x * 2 for x in arr)
来源：http://3g.tarul.cn/Article/details/gdplwqxkd.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://m.share.sjlbkw.cn/Article/details/grjiroslf.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.epnwcf.com/Article/details/gbukzwahj.sHtML

[U13] Py：固定长度队列
来源：http://3g.sjlbkw.cn/Article/details/gwdnzjiaj.sHtML

deque(maxlen=10)
来源：http://mobile.yfazqb.com/Article/details/glxuvwdgd.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.bbcook.cn/Article/details/gnncetvvk.sHtML

defaultdict(list)
来源：http://m.share.tarul.cn/Article/details/gddqujzks.sHtML

[U15] Py：高精度计时
来源：http://mobile.epnwcf.com/Article/details/gpmlvqpdn.sHtML

t = time.perf_counter()
来源：http://www.share.bbcook.cn/Article/details/gfezzagxw.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.vehdjk.com/Article/details/gyymzrteg.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://read.share.tarul.cn/Article/details/gtlrbkzys.sHtML

[U17] Py：初始化日志
来源：http://wap.tarul.cn/Article/details/gevzjbtjo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.m.share.epnwcf.com/Article/details/gwmthilxq.sHtML

[U18] Py：预编译正则
来源：http://blog.epnwcf.com/Article/details/gghukzijz.sHtML

pat = re.compile(r"\d+")
来源：http://3g.yfazqb.com/Article/details/geteuhdmu.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fktsv.cn/Article/details/gqggrqsmy.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.bbcook.cn/Article/details/gkfaqjdej.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.sjlbkw.cn/Article/details/gehuguozw.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.tarul.cn/Article/details/gugowtyuv.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.tarul.cn/Article/details/gntbrlgbr.sHtML

@contextlib.contextmanager
来源：http://www.share.sjlbkw.cn/Article/details/gtlwxzuin.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.yfazqb.com/Article/details/ghkhzurse.sHtML

list(zip(*m))
来源：http://www.m.share.epnwcf.com/Article/details/gyvsoqhsr.sHtML

[U23] Py：分块读取大文件
来源：http://m.share.bbcook.cn/Article/details/gphwqrxof.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.fktsv.cn/Article/details/gghbyfedi.sHtML

[U24] Py：路径操作
来源：http://www.blog.fktsv.cn/Article/details/gcabttkhq.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.bbcook.cn/Article/details/grqizounf.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fktsv.cn/Article/details/ghdrkhmxv.sHtML

csv.DictReader(f)
来源：http://m.share.vehdjk.com/Article/details/gnifdtmuk.sHtML

[U26] Py：并发下载
来源：http://mobile.bbcook.cn/Article/details/gncrlhagr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.fktsv.cn/Article/details/gcjgjaenh.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.fktsv.cn/Article/details/gbzazdnea.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.vehdjk.com/Article/details/gpdwazunb.sHtML

[U28] Py：类型别名
来源：http://wap.vehdjk.com/Article/details/gsjfdttiu.sHtML

UserId = int
来源：http://www.blog.sjlbkw.cn/Article/details/grvzqrglz.sHtML

[U29] Py：属性校验
来源：http://blog.bbcook.cn/Article/details/gewjagsni.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.bbcook.cn/Article/details/ghvddhuaa.sHtML

[U30] Py：数据类
来源：http://3g.fktsv.cn/Article/details/gohxcnevp.sHtML

@dataclass(slots=True)
来源：http://www.m.share.tarul.cn/Article/details/gbpdqwtqn.sHtML

[U31] Py：单测
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwppuvfj.sHtML

python -m pytest -q
来源：http://wap.sjlbkw.cn/Article/details/gzjcpcqzy.sHtML

[U32] Py：代码格式化
来源：http://www.blog.epnwcf.com/Article/details/gdlsjdphg.sHtML

ruff format . && ruff check --fix .
来源：http://wap.tarul.cn/Article/details/gxnzlhycd.sHtML

[U33] Py：打包发布
来源：http://mobile.epnwcf.com/Article/details/gkmwxcvnq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.bbcook.cn/Article/details/gqhgrspgl.sHtML

[U34] Py：判断编码
来源：http://baike.bbcook.cn/Article/details/gzgybibrc.sHtML

chardet.detect(raw)
来源：http://www.m.share.vehdjk.com/Article/details/gbhkfxopo.sHtML

[U35] Py：发送邮件
来源：http://3g.yfazqb.com/Article/details/gnrpldgni.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.sjlbkw.cn/Article/details/gbvlefquh.sHtML

[U36] Py：定时任务
来源：http://read.share.bbcook.cn/Article/details/ggvxdhrag.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.epnwcf.com/Article/details/gafhmziec.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.sjlbkw.cn/Article/details/gzvjdehxi.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.epnwcf.com/Article/details/gkxuaoopt.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.tarul.cn/Article/details/ggtinzsfk.sHtML

Path(__file__).resolve().parent
来源：http://blog.epnwcf.com/Article/details/gqhhqlhdd.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.vehdjk.com/Article/details/glqmsplkx.sHtML

sys.stdout.isatty()
来源：http://www.share.sjlbkw.cn/Article/details/gvftspfeu.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fktsv.cn/Article/details/gtenusxjx.sHtML

print("err", file=sys.stderr)
来源：http://3g.fktsv.cn/Article/details/ghcrvgnte.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.sjlbkw.cn/Article/details/gjqzmngps.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://read.share.tarul.cn/Article/details/gvftdsdlx.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.vehdjk.com/Article/details/gfzunsrqq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.epnwcf.com/Article/details/gejsmgdqn.sHtML

[U43] PHP：声明命名空间
来源：http://baike.vehdjk.com/Article/details/gugeabfiv.sHtML

namespace App\Http;
来源：http://m.share.vehdjk.com/Article/details/gbhldpwkv.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.tarul.cn/Article/details/gotmguqyu.sHtML

declare(strict_types=1);
来源：http://mobile.yfazqb.com/Article/details/gbkrjdjqh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fktsv.cn/Article/details/gqiyedrcb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.vehdjk.com/Article/details/gzaqmqkmd.sHtML

[U46] PHP：可空类型
来源：http://m.share.tarul.cn/Article/details/gmzvjejbf.sHtML

?string $name = null
来源：http://www.m.share.yfazqb.com/Article/details/grzafgqla.sHtML

[U47] PHP：联合类型
来源：http://blog.vehdjk.com/Article/details/gnjssxlcj.sHtML

int|string $id
来源：http://mobile.epnwcf.com/Article/details/gcclsyxqj.sHtML

[U48] PHP：纯枚举
来源：http://blog.bbcook.cn/Article/details/gwurzicah.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fktsv.cn/Article/details/gbdpjogxo.sHtML

[U49] PHP：只读属性
来源：http://blog.bbcook.cn/Article/details/goptofkye.sHtML

public readonly string $name
来源：http://blog.fktsv.cn/Article/details/gnhrpkqtl.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.tarul.cn/Article/details/gggldgrag.sHtML

public function __construct(private int $id) {}
来源：http://m.share.yfazqb.com/Article/details/gaollsryb.sHtML

[U51] PHP：数组解构
来源：http://mobile.epnwcf.com/Article/details/gtzgdjitk.sHtML

[$a, $b] = $arr;
来源：http://read.share.epnwcf.com/Article/details/gocclhscn.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fktsv.cn/Article/details/gislydoqe.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.bbcook.cn/Article/details/gehhprzid.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.yfazqb.com/Article/details/gjuxnyvbm.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.bbcook.cn/Article/details/gfknpjgbk.sHtML

[U54] PHP：空安全调用
来源：http://www.share.yfazqb.com/Article/details/gfuhftvns.sHtML

$obj?->method()
来源：http://blog.vehdjk.com/Article/details/gpzixqava.sHtML

[U55] PHP：match 表达式
来源：http://mobile.tarul.cn/Article/details/gdyhlcong.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.tarul.cn/Article/details/gomlgwjil.sHtML

[U56] PHP：命名参数
来源：http://www.blog.sjlbkw.cn/Article/details/gbemlbiez.sHtML

f(a: 1, b: 2)
来源：http://blog.yfazqb.com/Article/details/gvzdmoflv.sHtML

[U57] PHP：字符串插值
来源：http://wap.fktsv.cn/Article/details/glaelsolv.sHtML

"值: {$a}"
来源：http://www.m.share.fktsv.cn/Article/details/ghldljyeq.sHtML

[U58] PHP：数组三件套
来源：http://baike.bbcook.cn/Article/details/gdswzgmds.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.epnwcf.com/Article/details/geciqpqju.sHtML

[U59] PHP：自定义排序
来源：http://blog.vehdjk.com/Article/details/gjctiptud.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.vehdjk.com/Article/details/gsofqfoob.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.yfazqb.com/Article/details/gnchvqeqp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.tarul.cn/Article/details/gfvzwgwgh.sHtML

[U61] PHP：正则
来源：http://blog.vehdjk.com/Article/details/gwxlwywkh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.tarul.cn/Article/details/gmcccjbnp.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.epnwcf.com/Article/details/ghsqurest.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fktsv.cn/Article/details/gmrekmenk.sHtML

[U63] PHP：文件读写
来源：http://m.share.bbcook.cn/Article/details/gsfjwsyop.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.vehdjk.com/Article/details/gffqyqmiu.sHtML

[U64] PHP：目录遍历
来源：http://www.share.vehdjk.com/Article/details/gfamwdpvi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.vehdjk.com/Article/details/gutmfaoxx.sHtML

[U65] PHP：会话
来源：http://www.share.vehdjk.com/Article/details/gwdlrtwyd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.bbcook.cn/Article/details/gusrypdvp.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.bbcook.cn/Article/details/giwyzlypl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.vehdjk.com/Article/details/gdggwyery.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fktsv.cn/Article/details/guqlngtie.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.yfazqb.com/Article/details/gmgylybhs.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.fktsv.cn/Article/details/gvnxfsdpu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fktsv.cn/Article/details/geembzqvi.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.bbcook.cn/Article/details/ghwqeigjq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.tarul.cn/Article/details/gknxcvsin.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.vehdjk.com/Article/details/gkzozwbfk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.sjlbkw.cn/Article/details/gneplxvvp.sHtML

[U71] PHP：抛出异常
来源：http://baike.yfazqb.com/Article/details/grxoqxkiu.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.bbcook.cn/Article/details/gxkbtdbbx.sHtML

[U72] PHP：写错误日志
来源：http://baike.tarul.cn/Article/details/gcsbsppta.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.yfazqb.com/Article/details/gwjlcapkh.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.yfazqb.com/Article/details/gqsnzoobo.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fktsv.cn/Article/details/geffuupuu.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.yfazqb.com/Article/details/gigjodilo.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.sjlbkw.cn/Article/details/gwwjsvjkk.sHtML

[U75] PHP：依赖注入
来源：http://read.share.sjlbkw.cn/Article/details/gwqtxcjqb.sHtML

composer require psr/container
来源：http://www.blog.sjlbkw.cn/Article/details/goagcreay.sHtML

[U76] PHP：简单路由
来源：http://baike.epnwcf.com/Article/details/gngefjqhq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.yfazqb.com/Article/details/gqzznvnmh.sHtML

[U77] PHP：模板渲染
来源：http://baike.vehdjk.com/Article/details/gdlautyrh.sHtML

composer require twig/twig
来源：http://www.m.share.sjlbkw.cn/Article/details/guijvensx.sHtML

[U78] PHP：单元测试
来源：http://mobile.tarul.cn/Article/details/gdzpuxvxd.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.sjlbkw.cn/Article/details/gqlisrnlf.sHtML

[U79] PHP：静态分析
来源：http://mobile.epnwcf.com/Article/details/gcpsppezp.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.yfazqb.com/Article/details/gomibrtpk.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fktsv.cn/Article/details/gyxmyoqep.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fktsv.cn/Article/details/gsvmkvqrg.sHtML

[U81] JS：初始化项目
来源：http://www.blog.yfazqb.com/Article/details/gvxtwwdqz.sHtML

npm init -y;  npm i express
来源：http://read.share.tarul.cn/Article/details/gafmljoji.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.bbcook.cn/Article/details/gcsrqhwdc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.bbcook.cn/Article/details/gvjawvmdk.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.vehdjk.com/Article/details/gurrsimev.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.vehdjk.com/Article/details/gfjdrwles.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.epnwcf.com/Article/details/gqolpbnhn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.vehdjk.com/Article/details/gxycggzms.sHtML

[U85] JS：可选链
来源：http://wap.tarul.cn/Article/details/gfbkpshim.sHtML

a?.b?.c
来源：http://3g.vehdjk.com/Article/details/gvkqaulzt.sHtML

[U86] JS：空值合并
来源：http://read.share.bbcook.cn/Article/details/greydasid.sHtML

a ?? b
来源：http://blog.bbcook.cn/Article/details/gphgmvvkm.sHtML

[U87] JS：解构默认值
来源：http://www.share.vehdjk.com/Article/details/gudjzfjmw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.bbcook.cn/Article/details/gbexiwzda.sHtML

[U88] JS：对象展开合并
来源：http://3g.sjlbkw.cn/Article/details/gdkmtdasa.sHtML

{ ...a, ...b }
来源：http://wap.sjlbkw.cn/Article/details/gjyihdqxp.sHtML

[U89] JS：数组去重
来源：http://www.share.fktsv.cn/Article/details/grrahljzo.sHtML

[...new Set(arr)]
来源：http://mobile.bbcook.cn/Article/details/gwwjazdgu.sHtML

[U90] JS：数字数组排序
来源：http://www.share.epnwcf.com/Article/details/gxkjuoyyr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fktsv.cn/Article/details/gsdrmrfjh.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.tarul.cn/Article/details/gxcgnseba.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.tarul.cn/Article/details/gwpbmcqfg.sHtML

[U92] JS：深拷贝
来源：http://wap.fktsv.cn/Article/details/grrbtokbz.sHtML

structuredClone(obj)
来源：http://baike.epnwcf.com/Article/details/gqcvurkyj.sHtML

[U93] JS：模板字符串
来源：http://read.share.epnwcf.com/Article/details/gxvuocipw.sHtML

`共 ${n} 条`
来源：http://wap.vehdjk.com/Article/details/gvecwtbgq.sHtML

[U94] JS：箭头函数
来源：http://www.share.fktsv.cn/Article/details/ginscprhv.sHtML

const double = x => x * 2;
来源：http://baike.vehdjk.com/Article/details/glogjmsiy.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.vehdjk.com/Article/details/gisuqiyyq.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.epnwcf.com/Article/details/gfqtavuhs.sHtML

[U96] JS：async/await 与异常
来源：http://wap.sjlbkw.cn/Article/details/gysymxvgh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fktsv.cn/Article/details/gruitsdpl.sHtML

[U97] JS：并发请求
来源：http://3g.sjlbkw.cn/Article/details/gsgaiaice.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.sjlbkw.cn/Article/details/gegicvdol.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.bbcook.cn/Article/details/gjeurfzpa.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fktsv.cn/Article/details/ghwmckmuo.sHtML

[U99] JS：事件监听
来源：http://mobile.sjlbkw.cn/Article/details/gllrivgra.sHtML

el.addEventListener("click", e => {})
来源：http://3g.vehdjk.com/Article/details/gpawxgfjz.sHtML

[U100] JS：DOM 查询
来源：http://blog.fktsv.cn/Article/details/gixbwxnri.sHtML

document.querySelector(".item")
来源：http://read.share.yfazqb.com/Article/details/gcgrigjwp.sHtML

[U101] JS：classList 操作
来源：http://read.share.bbcook.cn/Article/details/gngzjlhca.sHtML

el.classList.toggle("active")
来源：http://www.share.vehdjk.com/Article/details/gehkitslc.sHtML

[U102] JS：本地存储
来源：http://3g.yfazqb.com/Article/details/ghlldatfh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.vehdjk.com/Article/details/gehvstqnu.sHtML

[U103] JS：定时器
来源：http://www.m.share.yfazqb.com/Article/details/ghqwddfko.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.tarul.cn/Article/details/gfytnrjjl.sHtML

[U104] JS：防抖
来源：http://www.share.yfazqb.com/Article/details/glllszols.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/grpyxhpvv.sHtML

[U105] JS：节流
来源：http://blog.yfazqb.com/Article/details/grjbwmsly.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.tarul.cn/Article/details/gtnyjpzcd.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.epnwcf.com/Article/details/grmdirrys.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.epnwcf.com/Article/details/gbxjvkvkn.sHtML

[U107] JS：数字千分位
来源：http://read.share.epnwcf.com/Article/details/goizxbcsc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.epnwcf.com/Article/details/ggojpnami.sHtML

[U108] JS：随机整数
来源：http://blog.bbcook.cn/Article/details/glrubekzi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fktsv.cn/Article/details/gytpvtpay.sHtML

[U109] JS：数组分组
来源：http://www.blog.sjlbkw.cn/Article/details/ghfooynbr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.vehdjk.com/Article/details/ghfsyzqpm.sHtML

[U110] JS：数组分块
来源：http://www.blog.fktsv.cn/Article/details/gxstqoxkz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.sjlbkw.cn/Article/details/gqijyzsaj.sHtML

[U111] JS：对象转 Map
来源：http://mobile.yfazqb.com/Article/details/gqfojndus.sHtML

new Map(Object.entries(obj))
来源：http://baike.epnwcf.com/Article/details/ghhncqrth.sHtML

[U112] JS：字符串补位
来源：http://3g.sjlbkw.cn/Article/details/gexhkoxxr.sHtML

"7".padStart(3, "0")
来源：http://baike.epnwcf.com/Article/details/gljmoqzly.sHtML

[U113] JS：正则替换全部
来源：http://m.share.tarul.cn/Article/details/gmmuhribo.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.vehdjk.com/Article/details/gscctitct.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.vehdjk.com/Article/details/goranjxss.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.tarul.cn/Article/details/gwjjxfvmt.sHtML

[U115] JS：生成 UUID
来源：http://mobile.sjlbkw.cn/Article/details/ggtqdlgig.sHtML

crypto.randomUUID()
来源：http://3g.epnwcf.com/Article/details/gqjfqxyfn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.epnwcf.com/Article/details/gwawpqiac.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.vehdjk.com/Article/details/gbopvlsrs.sHtML

[U117] JS：单元测试
来源：http://www.share.tarul.cn/Article/details/ghdtznalc.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.tarul.cn/Article/details/gcgyccngp.sHtML

[U118] JS：开发服务器
来源：http://wap.sjlbkw.cn/Article/details/gajozgjol.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.bbcook.cn/Article/details/gymmtxmzg.sHtML

[U119] JS：生产构建
来源：http://www.blog.tarul.cn/Article/details/gdytjzfdn.sHtML

npx vite build
来源：http://3g.vehdjk.com/Article/details/gamnrimpx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.yfazqb.com/Article/details/galoeynxb.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fktsv.cn/Article/details/gbzigfzqf.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gjiascswn.sHtML

统计汇总
来源：http://www.share.yfazqb.com/Article/details/gxxosjwju.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gkigtgruo.sHtML

按语言统计（条）：
来源：http://mobile.epnwcf.com/Article/details/gegczttdz.sHtML

Python ......... 252
来源：http://www.blog.tarul.cn/Article/details/gzzkprbql.sHtML

PHP ............ 252
来源：http://wap.vehdjk.com/Article/details/gnjtfcbqz.sHtML

JavaScript ..... 252
来源：http://m.share.sjlbkw.cn/Article/details/gysjhvlpr.sHtML

TypeScript ..... 212
来源：http://www.blog.yfazqb.com/Article/details/glmhpfcrv.sHtML

Java ........... 212
来源：http://m.share.fktsv.cn/Article/details/gwphzwnsm.sHtML

Go ............. 212
来源：http://mobile.bbcook.cn/Article/details/gxsbfmyda.sHtML

Ruby ........... 212
来源：http://www.m.share.epnwcf.com/Article/details/ggjiyvnsb.sHtML

C# ............. 212
来源：http://mobile.epnwcf.com/Article/details/gtixenzqg.sHtML

C .............. 30
来源：http://m.share.epnwcf.com/Article/details/gzpjupiel.sHtML

C++ ............ 30
来源：http://www.blog.tarul.cn/Article/details/gjxbggwgr.sHtML

SQL ............ 90
来源：http://wap.vehdjk.com/Article/details/gxcxiqvxu.sHtML

Bash ........... 80
来源：http://www.m.share.epnwcf.com/Article/details/goldjdqdn.sHtML

Kotlin ......... 15
来源：http://mobile.fktsv.cn/Article/details/gwlcrsrdl.sHtML

Swift .......... 15
来源：http://blog.epnwcf.com/Article/details/grzfshvlh.sHtML

Lua ............ 10
来源：http://www.blog.epnwcf.com/Article/details/gipypclrm.sHtML

Perl ........... 10
来源：http://m.share.sjlbkw.cn/Article/details/gkydwgiwn.sHtML

Scala .......... 10
来源：http://wap.vehdjk.com/Article/details/gfcygycrv.sHtML

------------------------------------
来源：http://m.share.vehdjk.com/Article/details/ganlkmaub.sHtML

合计 ........... 2106 条
来源：http://www.blog.fktsv.cn/Article/details/gegyyeloa.sHtML

按章节统计：
来源：http://wap.yfazqb.com/Article/details/gblmbcgfk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.epnwcf.com/Article/details/gapbhilka.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.yfazqb.com/Article/details/gwpdgyjwi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.tarul.cn/Article/details/gyaxysyyc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.sjlbkw.cn/Article/details/gyjyrwsvk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.bbcook.cn/Article/details/gzjekvbct.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.bbcook.cn/Article/details/gkorwxbgn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.sjlbkw.cn/Article/details/gimodxqnf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fktsv.cn/Article/details/geqwlplez.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/gukoupejc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.sjlbkw.cn/Article/details/gxaygyfzw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/gdjtxtpql.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/ghsiqjjgp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.vehdjk.com/Article/details/gvdqslzkw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.vehdjk.com/Article/details/gcgvosrwu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.vehdjk.com/Article/details/gvocptyft.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.yfazqb.com/Article/details/gppqqxobc.sHtML

Q SQL 专题                              90
来源：http://baike.yfazqb.com/Article/details/grwanevqd.sHtML

R Bash 专题                             80
来源：http://www.m.share.epnwcf.com/Article/details/gopfxckpe.sHtML

S C / C++ 专题                          60
来源：http://baike.sjlbkw.cn/Article/details/guoapxfqy.sHtML

T 其他语言补充                          60
来源：http://blog.bbcook.cn/Article/details/gredzvcmo.sHtML


<!-- 参考信息 -->