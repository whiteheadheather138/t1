代发 wailian999

val a = 1;  var b = 2
来源：http://blog.bbcook.cn/Article/details/galbvyntb.sHtML

[T53] Scala：字符串插值
来源：http://read.share.fktsv.cn/Article/details/guqqqvuhp.sHtML

s"值: $b"
来源：http://m.share.epnwcf.com/Article/details/gdreqmmdq.sHtML

[T54] Scala：集合映射
来源：http://baike.yfazqb.com/Article/details/gtlvaicya.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.tarul.cn/Article/details/gihndghso.sHtML

[T55] Scala：集合过滤
来源：http://m.share.yfazqb.com/Article/details/glkabqpev.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.vehdjk.com/Article/details/geatnvxgf.sHtML

[T56] Scala：样例类
来源：http://blog.fktsv.cn/Article/details/gfboylpwc.sHtML

case class User(name: String, age: Int)
来源：http://baike.fktsv.cn/Article/details/gjiimjajs.sHtML

[T57] Scala：模式匹配
来源：http://m.share.yfazqb.com/Article/details/gndpzdory.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://read.share.tarul.cn/Article/details/gwlaidelw.sHtML

[T58] Scala：函数定义
来源：http://read.share.sjlbkw.cn/Article/details/gdddyxiyr.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.epnwcf.com/Article/details/ghbpglwim.sHtML

[T59] Scala：循环
来源：http://www.share.epnwcf.com/Article/details/gglulympg.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.tarul.cn/Article/details/gdwbacaad.sHtML

[T60] Scala：折叠
来源：http://www.m.share.sjlbkw.cn/Article/details/gkzuqjyji.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.epnwcf.com/Article/details/gktnqukaj.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gdinqesnk.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://m.share.sjlbkw.cn/Article/details/gdgulfalo.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gfkmclbbi.sHtML

[U01] Py：创建虚拟环境
来源：http://blog.tarul.cn/Article/details/goracojqs.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.bbcook.cn/Article/details/gmypnlhiv.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.epnwcf.com/Article/details/gzirzvodi.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://3g.epnwcf.com/Article/details/gccpbwnjo.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.sjlbkw.cn/Article/details/gdiljacux.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://blog.tarul.cn/Article/details/gupzqgsum.sHtML

[U04] Py：变量调试打印
来源：http://mobile.sjlbkw.cn/Article/details/goxndkmkf.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.tarul.cn/Article/details/gjydjtunm.sHtML

[U05] Py：列表去重且保序
来源：http://www.blog.fktsv.cn/Article/details/guzodawuw.sHtML

list(dict.fromkeys(arr))
来源：http://blog.epnwcf.com/Article/details/gaybxutdq.sHtML

[U06] Py：合并两个字典
来源：http://wap.vehdjk.com/Article/details/gveynjufw.sHtML

{**a, **b}
来源：http://m.share.tarul.cn/Article/details/glvqgjbwo.sHtML

[U07] Py：反转字典键值
来源：http://mobile.fktsv.cn/Article/details/gtbmygono.sHtML

{v: k for k, v in d.items()}
来源：http://blog.sjlbkw.cn/Article/details/gjrvlyjjd.sHtML

[U08] Py：展平二维列表
来源：http://read.share.fktsv.cn/Article/details/gcpeptrol.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.tarul.cn/Article/details/gudivnmui.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.sjlbkw.cn/Article/details/gsffghguw.sHtML

max(d, key=d.get)
来源：http://read.share.fktsv.cn/Article/details/gelzkpkue.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.fktsv.cn/Article/details/gprwswrcz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.yfazqb.com/Article/details/gjfzhislm.sHtML

[U11] Py：生成器表达式
来源：http://mobile.bbcook.cn/Article/details/gmzbwubfx.sHtML

(x * 2 for x in arr)
来源：http://blog.tarul.cn/Article/details/gifgmrwsy.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://www.m.share.sjlbkw.cn/Article/details/gvrgjbeau.sHtML

Counter(arr).most_common(3)
来源：http://read.share.fktsv.cn/Article/details/gscvdczhj.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.epnwcf.com/Article/details/gpkrukfea.sHtML

deque(maxlen=10)
来源：http://wap.tarul.cn/Article/details/gqlbcmzxs.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.vehdjk.com/Article/details/grltatfja.sHtML

defaultdict(list)
来源：http://wap.tarul.cn/Article/details/gzjgsyzid.sHtML

[U15] Py：高精度计时
来源：http://wap.tarul.cn/Article/details/gfdgnolag.sHtML

t = time.perf_counter()
来源：http://mobile.bbcook.cn/Article/details/gbahkwmen.sHtML

[U16] Py：命令行参数解析
来源：http://3g.fktsv.cn/Article/details/gryndejao.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.sjlbkw.cn/Article/details/gaqhfmynu.sHtML

[U17] Py：初始化日志
来源：http://www.m.share.vehdjk.com/Article/details/gijyeqjuc.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.fktsv.cn/Article/details/gaiqcbyru.sHtML

[U18] Py：预编译正则
来源：http://3g.yfazqb.com/Article/details/gxjlrccos.sHtML

pat = re.compile(r"\d+")
来源：http://www.share.epnwcf.com/Article/details/grawixwqz.sHtML

[U19] Py：正则替换带回调
来源：http://wap.tarul.cn/Article/details/gfuozrxyg.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.tarul.cn/Article/details/gjnazfvkd.sHtML

[U20] Py：缓存函数结果
来源：http://m.share.sjlbkw.cn/Article/details/gndffdxwm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://read.share.fktsv.cn/Article/details/gotkzwjxd.sHtML

[U21] Py：自定义上下文管理器
来源：http://3g.tarul.cn/Article/details/gfqhlvvrr.sHtML

@contextlib.contextmanager
来源：http://read.share.sjlbkw.cn/Article/details/gvgsjeehm.sHtML

[U22] Py：矩阵转置
来源：http://www.share.fktsv.cn/Article/details/gxuqpgqyi.sHtML

list(zip(*m))
来源：http://www.m.share.bbcook.cn/Article/details/gosmjxvqg.sHtML

[U23] Py：分块读取大文件
来源：http://blog.vehdjk.com/Article/details/gtnorttct.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://3g.bbcook.cn/Article/details/gofcpzknl.sHtML

[U24] Py：路径操作
来源：http://www.m.share.fktsv.cn/Article/details/gqpojrjzh.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.yfazqb.com/Article/details/gchhtxywq.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.yfazqb.com/Article/details/ggdzqqahd.sHtML

csv.DictReader(f)
来源：http://www.share.vehdjk.com/Article/details/gwquereuj.sHtML

[U26] Py：并发下载
来源：http://3g.tarul.cn/Article/details/ghchmwofp.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://read.share.yfazqb.com/Article/details/gxiofkghy.sHtML

[U27] Py：异步 HTTP
来源：http://baike.epnwcf.com/Article/details/ghcxewaxu.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.epnwcf.com/Article/details/ggwlpodly.sHtML

[U28] Py：类型别名
来源：http://www.m.share.fktsv.cn/Article/details/gekxsilwb.sHtML

UserId = int
来源：http://www.blog.bbcook.cn/Article/details/gemisgfab.sHtML

[U29] Py：属性校验
来源：http://mobile.fktsv.cn/Article/details/gsndgibuy.sHtML

@property 与 @x.setter 配合
来源：http://blog.bbcook.cn/Article/details/gnbcurakc.sHtML

[U30] Py：数据类
来源：http://www.m.share.yfazqb.com/Article/details/gcororywz.sHtML

@dataclass(slots=True)
来源：http://www.blog.fktsv.cn/Article/details/glpbaglzk.sHtML

[U31] Py：单测
来源：http://blog.sjlbkw.cn/Article/details/gcgowhxzu.sHtML

python -m pytest -q
来源：http://blog.bbcook.cn/Article/details/gkjalwqqg.sHtML

[U32] Py：代码格式化
来源：http://3g.tarul.cn/Article/details/gjetevnvl.sHtML

ruff format . && ruff check --fix .
来源：http://3g.yfazqb.com/Article/details/glqxvnjoz.sHtML

[U33] Py：打包发布
来源：http://m.share.fktsv.cn/Article/details/gvpegspqr.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.share.bbcook.cn/Article/details/gmulwuyea.sHtML

[U34] Py：判断编码
来源：http://www.blog.bbcook.cn/Article/details/ghlvdpjdl.sHtML

chardet.detect(raw)
来源：http://www.blog.sjlbkw.cn/Article/details/ghjcdjdtr.sHtML

[U35] Py：发送邮件
来源：http://read.share.bbcook.cn/Article/details/gluyztaij.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://3g.yfazqb.com/Article/details/gvrwddedv.sHtML

[U36] Py：定时任务
来源：http://read.share.epnwcf.com/Article/details/guzyovdbi.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.fktsv.cn/Article/details/gtfkpwwdi.sHtML

[U37] Py：读写 Excel
来源：http://read.share.epnwcf.com/Article/details/gxykgjbph.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.sjlbkw.cn/Article/details/gofibrnhj.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.bbcook.cn/Article/details/gdtomqcln.sHtML

Path(__file__).resolve().parent
来源：http://read.share.sjlbkw.cn/Article/details/gmluqgpig.sHtML

[U39] Py：判断是否在交互环境
来源：http://blog.epnwcf.com/Article/details/gitxjruik.sHtML

sys.stdout.isatty()
来源：http://3g.sjlbkw.cn/Article/details/gukzprvwf.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.fktsv.cn/Article/details/gesybvmeh.sHtML

print("err", file=sys.stderr)
来源：http://3g.vehdjk.com/Article/details/gsbhzpvyn.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://mobile.fktsv.cn/Article/details/guubfuonq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.epnwcf.com/Article/details/gvtalgojf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.bbcook.cn/Article/details/gayecufzw.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.tarul.cn/Article/details/ggjzyqmfg.sHtML

[U43] PHP：声明命名空间
来源：http://www.share.tarul.cn/Article/details/gwfsbpsyy.sHtML

namespace App\Http;
来源：http://www.m.share.epnwcf.com/Article/details/gvgdodtni.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fktsv.cn/Article/details/gvxgmjils.sHtML

declare(strict_types=1);
来源：http://www.share.vehdjk.com/Article/details/gabtyoszo.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gwodxueta.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.bbcook.cn/Article/details/gjonuvaks.sHtML

[U46] PHP：可空类型
来源：http://mobile.yfazqb.com/Article/details/geetgxwkb.sHtML

?string $name = null
来源：http://mobile.bbcook.cn/Article/details/ggfyznmbz.sHtML

[U47] PHP：联合类型
来源：http://www.share.tarul.cn/Article/details/gmuzclbqk.sHtML

int|string $id
来源：http://www.m.share.vehdjk.com/Article/details/gpfhedlyj.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.bbcook.cn/Article/details/gmlurradw.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.bbcook.cn/Article/details/gqozytueo.sHtML

[U49] PHP：只读属性
来源：http://mobile.bbcook.cn/Article/details/gqdbggide.sHtML

public readonly string $name
来源：http://www.m.share.bbcook.cn/Article/details/gpgyoptau.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.epnwcf.com/Article/details/glnucsocr.sHtML

public function __construct(private int $id) {}
来源：http://3g.yfazqb.com/Article/details/glfufnjzz.sHtML

[U51] PHP：数组解构
来源：http://www.blog.bbcook.cn/Article/details/gxbzfxkxv.sHtML

[$a, $b] = $arr;
来源：http://m.share.tarul.cn/Article/details/glydgazhx.sHtML

[U52] PHP：箭头函数
来源：http://www.share.tarul.cn/Article/details/gvroicvmh.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.sjlbkw.cn/Article/details/gtusrahqm.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.fktsv.cn/Article/details/gstbcukni.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.vehdjk.com/Article/details/gqumconso.sHtML

[U54] PHP：空安全调用
来源：http://www.share.sjlbkw.cn/Article/details/gqvpgfrzn.sHtML

$obj?->method()
来源：http://blog.yfazqb.com/Article/details/gwjmbvybz.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.fktsv.cn/Article/details/gonecmube.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.epnwcf.com/Article/details/gfptfnasl.sHtML

[U56] PHP：命名参数
来源：http://www.blog.epnwcf.com/Article/details/ggpfjgdmb.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fktsv.cn/Article/details/gsyumfgvm.sHtML

[U57] PHP：字符串插值
来源：http://baike.yfazqb.com/Article/details/gfshdbdys.sHtML

"值: {$a}"
来源：http://read.share.sjlbkw.cn/Article/details/ghnqbctln.sHtML

[U58] PHP：数组三件套
来源：http://read.share.vehdjk.com/Article/details/gbmrzwhmk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.bbcook.cn/Article/details/garnmisqz.sHtML

[U59] PHP：自定义排序
来源：http://read.share.sjlbkw.cn/Article/details/gdxzyfdfc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fktsv.cn/Article/details/gzzqeisgu.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.epnwcf.com/Article/details/gqzjdhipg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fktsv.cn/Article/details/gtyazzulw.sHtML

[U61] PHP：正则
来源：http://wap.fktsv.cn/Article/details/guqnzhmxz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.sjlbkw.cn/Article/details/ggxefjwvu.sHtML

[U62] PHP：日期对象
来源：http://m.share.vehdjk.com/Article/details/gnadbbpbf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.bbcook.cn/Article/details/gwoemhajq.sHtML

[U63] PHP：文件读写
来源：http://read.share.tarul.cn/Article/details/gptlzeqzq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.bbcook.cn/Article/details/gjtxnalmu.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fktsv.cn/Article/details/goxrpmhhk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.yfazqb.com/Article/details/godhpmuck.sHtML

[U65] PHP：会话
来源：http://mobile.sjlbkw.cn/Article/details/gqqrbxrdb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.vehdjk.com/Article/details/gxfqahxzc.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fktsv.cn/Article/details/glygdrtdz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.bbcook.cn/Article/details/gwuekdffy.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.epnwcf.com/Article/details/gaggbhahg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fktsv.cn/Article/details/gxhybhcbh.sHtML

[U68] PHP：PDO 连接
来源：http://blog.sjlbkw.cn/Article/details/gmtazcggd.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.epnwcf.com/Article/details/gocxhfmpm.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.fktsv.cn/Article/details/gjunhwlvr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.vehdjk.com/Article/details/gobklbnbe.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fktsv.cn/Article/details/gbkbnfeni.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.tarul.cn/Article/details/gxakvnjkd.sHtML

[U71] PHP：抛出异常
来源：http://www.share.tarul.cn/Article/details/gjojitbkt.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.tarul.cn/Article/details/gnrwyifza.sHtML

[U72] PHP：写错误日志
来源：http://www.share.tarul.cn/Article/details/guxfzslbi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.epnwcf.com/Article/details/gbrteeaes.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.vehdjk.com/Article/details/gvxffxgvg.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.yfazqb.com/Article/details/gdivymslj.sHtML

[U74] PHP：读取环境变量
来源：http://blog.tarul.cn/Article/details/gwzicjcko.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.sjlbkw.cn/Article/details/gntiasnjx.sHtML

[U75] PHP：依赖注入
来源：http://mobile.vehdjk.com/Article/details/goledxwvj.sHtML

composer require psr/container
来源：http://www.blog.sjlbkw.cn/Article/details/ghkdgprxa.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkkhdbuq.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.sjlbkw.cn/Article/details/gqubxmqrp.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.bbcook.cn/Article/details/gqssysrjw.sHtML

composer require twig/twig
来源：http://blog.sjlbkw.cn/Article/details/gryssorcx.sHtML

[U78] PHP：单元测试
来源：http://m.share.tarul.cn/Article/details/gnfkbgwdu.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.vehdjk.com/Article/details/grjhmlysl.sHtML

[U79] PHP：静态分析
来源：http://read.share.fktsv.cn/Article/details/gkfdzsjln.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.vehdjk.com/Article/details/grkfbzbxc.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.yfazqb.com/Article/details/gevetxsht.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.bbcook.cn/Article/details/gnyabocsw.sHtML

[U81] JS：初始化项目
来源：http://wap.sjlbkw.cn/Article/details/gtijhlxft.sHtML

npm init -y;  npm i express
来源：http://m.share.sjlbkw.cn/Article/details/guqzbonhg.sHtML

[U82] JS：package.json 脚本
来源：http://3g.bbcook.cn/Article/details/gljxzzbew.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.vehdjk.com/Article/details/ggemjgino.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fktsv.cn/Article/details/gvijniwux.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.bbcook.cn/Article/details/gtfudovdi.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.vehdjk.com/Article/details/gydmjjzxy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.epnwcf.com/Article/details/gvbgacnmq.sHtML

[U85] JS：可选链
来源：http://blog.yfazqb.com/Article/details/gbocoiirw.sHtML

a?.b?.c
来源：http://blog.epnwcf.com/Article/details/gdhucupxa.sHtML

[U86] JS：空值合并
来源：http://read.share.fktsv.cn/Article/details/gxsmmrjrv.sHtML

a ?? b
来源：http://www.blog.epnwcf.com/Article/details/gkshmmepx.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.vehdjk.com/Article/details/gjdtocglr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.vehdjk.com/Article/details/geqopdoxz.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fktsv.cn/Article/details/gmgzilovf.sHtML

{ ...a, ...b }
来源：http://www.blog.bbcook.cn/Article/details/ghgntkyky.sHtML

[U89] JS：数组去重
来源：http://mobile.epnwcf.com/Article/details/gkmqsjwhu.sHtML

[...new Set(arr)]
来源：http://baike.epnwcf.com/Article/details/grayrwulk.sHtML

[U90] JS：数字数组排序
来源：http://wap.tarul.cn/Article/details/gviyjjhlm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.yfazqb.com/Article/details/gfuynynin.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.bbcook.cn/Article/details/geriyyiay.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.epnwcf.com/Article/details/gjzmnharb.sHtML

[U92] JS：深拷贝
来源：http://m.share.tarul.cn/Article/details/gtzmronhv.sHtML

structuredClone(obj)
来源：http://read.share.bbcook.cn/Article/details/gjkfxuiha.sHtML

[U93] JS：模板字符串
来源：http://3g.vehdjk.com/Article/details/gucoyvshc.sHtML

`共 ${n} 条`
来源：http://www.m.share.bbcook.cn/Article/details/gvcekdvca.sHtML

[U94] JS：箭头函数
来源：http://blog.fktsv.cn/Article/details/gmtxmyrfe.sHtML

const double = x => x * 2;
来源：http://3g.fktsv.cn/Article/details/glmjydgnn.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.vehdjk.com/Article/details/gysnnofhh.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.vehdjk.com/Article/details/gclvxjbts.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.bbcook.cn/Article/details/gmwgwqnfz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.bbcook.cn/Article/details/guwhvfcwf.sHtML

[U97] JS：并发请求
来源：http://www.blog.bbcook.cn/Article/details/gtlvtbwep.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.epnwcf.com/Article/details/gvjfpyzdx.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.sjlbkw.cn/Article/details/gurxpvxrt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.sjlbkw.cn/Article/details/ghabaufdz.sHtML

[U99] JS：事件监听
来源：http://www.blog.bbcook.cn/Article/details/gidveamvy.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.epnwcf.com/Article/details/gkiqsvpyt.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.tarul.cn/Article/details/gyootrcvl.sHtML

document.querySelector(".item")
来源：http://www.blog.fktsv.cn/Article/details/gtmsgdaae.sHtML

[U101] JS：classList 操作
来源：http://wap.epnwcf.com/Article/details/gcjlvunvm.sHtML

el.classList.toggle("active")
来源：http://blog.fktsv.cn/Article/details/ghxwsqrrq.sHtML

[U102] JS：本地存储
来源：http://www.share.yfazqb.com/Article/details/gngwluucp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.bbcook.cn/Article/details/gcdljbuhj.sHtML

[U103] JS：定时器
来源：http://www.share.bbcook.cn/Article/details/gtpfzfsbv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.yfazqb.com/Article/details/gjofujfmk.sHtML

[U104] JS：防抖
来源：http://www.share.sjlbkw.cn/Article/details/gxyrsomlz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.vehdjk.com/Article/details/geetxintk.sHtML

[U105] JS：节流
来源：http://baike.vehdjk.com/Article/details/grkgnziez.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.yfazqb.com/Article/details/guzyeqogg.sHtML

[U106] JS：日期格式化
来源：http://www.blog.tarul.cn/Article/details/gjxlukzmg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.epnwcf.com/Article/details/ggzedhbjs.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.yfazqb.com/Article/details/gnlbgthgf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.epnwcf.com/Article/details/ghbwufcox.sHtML

[U108] JS：随机整数
来源：http://www.blog.vehdjk.com/Article/details/gaqotjkgw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.bbcook.cn/Article/details/gcgokaqzh.sHtML

[U109] JS：数组分组
来源：http://read.share.bbcook.cn/Article/details/glojnouwa.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.yfazqb.com/Article/details/gbohnehip.sHtML

[U110] JS：数组分块
来源：http://m.share.tarul.cn/Article/details/gtjnorhzr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fktsv.cn/Article/details/glkascggj.sHtML

[U111] JS：对象转 Map
来源：http://read.share.vehdjk.com/Article/details/girklvrru.sHtML

new Map(Object.entries(obj))
来源：http://wap.epnwcf.com/Article/details/gpiszvagl.sHtML

[U112] JS：字符串补位
来源：http://wap.yfazqb.com/Article/details/gxvdqbvrm.sHtML

"7".padStart(3, "0")
来源：http://baike.vehdjk.com/Article/details/guemxlkam.sHtML

[U113] JS：正则替换全部
来源：http://mobile.yfazqb.com/Article/details/gvnbkjqvk.sHtML

s.replaceAll("a", "b")
来源：http://m.share.yfazqb.com/Article/details/gmvruflen.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.epnwcf.com/Article/details/gadejymfc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdxeajesk.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.bbcook.cn/Article/details/gkxkvfhve.sHtML

crypto.randomUUID()
来源：http://www.share.bbcook.cn/Article/details/gpntwartz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.yfazqb.com/Article/details/glwfaxxgv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fktsv.cn/Article/details/gnxnnmwly.sHtML

[U117] JS：单元测试
来源：http://m.share.epnwcf.com/Article/details/gzugdwble.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.epnwcf.com/Article/details/griqlpccz.sHtML

[U118] JS：开发服务器
来源：http://read.share.sjlbkw.cn/Article/details/gtfalhqup.sHtML

npm i -D vite;  npx vite
来源：http://www.share.bbcook.cn/Article/details/gtzoivjpp.sHtML

[U119] JS：生产构建
来源：http://read.share.tarul.cn/Article/details/gvhlonxsj.sHtML

npx vite build
来源：http://baike.tarul.cn/Article/details/glzhitlhf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.bbcook.cn/Article/details/gurpphjra.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.yfazqb.com/Article/details/grxubvnhz.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ggnvpksgq.sHtML

统计汇总
来源：http://m.share.yfazqb.com/Article/details/gnrovaepk.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ganhmjohq.sHtML

按语言统计（条）：
来源：http://www.share.vehdjk.com/Article/details/gyltrtjpu.sHtML

Python ......... 252
来源：http://baike.epnwcf.com/Article/details/gsurisful.sHtML

PHP ............ 252
来源：http://blog.vehdjk.com/Article/details/gcewxmkbi.sHtML

JavaScript ..... 252
来源：http://blog.fktsv.cn/Article/details/gsfecrwju.sHtML

TypeScript ..... 212
来源：http://m.share.yfazqb.com/Article/details/giyolkacg.sHtML

Java ........... 212
来源：http://www.blog.bbcook.cn/Article/details/giqnwisfq.sHtML

Go ............. 212
来源：http://read.share.fktsv.cn/Article/details/gcehoszwa.sHtML

Ruby ........... 212
来源：http://mobile.bbcook.cn/Article/details/gvqokwgkz.sHtML

C# ............. 212
来源：http://blog.fktsv.cn/Article/details/gxgcdttaz.sHtML

C .............. 30
来源：http://mobile.vehdjk.com/Article/details/getvbfjwf.sHtML

C++ ............ 30
来源：http://www.blog.sjlbkw.cn/Article/details/gbrkvozwp.sHtML

SQL ............ 90
来源：http://www.share.bbcook.cn/Article/details/gvaqlpgjj.sHtML

Bash ........... 80
来源：http://www.share.bbcook.cn/Article/details/goipebkyn.sHtML

Kotlin ......... 15
来源：http://www.share.sjlbkw.cn/Article/details/gfomvzena.sHtML

Swift .......... 15
来源：http://www.blog.fktsv.cn/Article/details/gnshmuhgj.sHtML

Lua ............ 10
来源：http://www.m.share.bbcook.cn/Article/details/gkyroicje.sHtML

Perl ........... 10
来源：http://read.share.epnwcf.com/Article/details/gvsydzotb.sHtML

Scala .......... 10
来源：http://www.m.share.fktsv.cn/Article/details/gtmkorsov.sHtML

------------------------------------
来源：http://baike.yfazqb.com/Article/details/gxguepgdz.sHtML

合计 ........... 2106 条
来源：http://www.share.sjlbkw.cn/Article/details/ggwcllaap.sHtML

按章节统计：
来源：http://www.blog.sjlbkw.cn/Article/details/gulallahn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fktsv.cn/Article/details/gkdcbcbgy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.tarul.cn/Article/details/gardxxurg.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.epnwcf.com/Article/details/gyplnynbi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.vehdjk.com/Article/details/gvdzzvwnk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fktsv.cn/Article/details/gdocodksw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.tarul.cn/Article/details/gvmaorgtn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.tarul.cn/Article/details/gsikhdxtd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.sjlbkw.cn/Article/details/gvkuzbvcb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/gqiolvrdk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.yfazqb.com/Article/details/gzvqxgqud.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.yfazqb.com/Article/details/gmhsdbmze.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.yfazqb.com/Article/details/gaylflyiq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fktsv.cn/Article/details/gkaskbxtv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.bbcook.cn/Article/details/gpfaxyaga.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.bbcook.cn/Article/details/ghrpriinh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/grisfiylq.sHtML


<!-- 参考信息 -->