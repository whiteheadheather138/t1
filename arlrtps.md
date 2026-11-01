代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://www.share.fktsv.cn/Article/details/gtwxnkxor.sHtML

[T55] Scala：集合过滤
来源：http://www.share.sjlbkw.cn/Article/details/gykejchhh.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.yfazqb.com/Article/details/gcknwurgy.sHtML

[T56] Scala：样例类
来源：http://www.share.sjlbkw.cn/Article/details/gopkarbvp.sHtML

case class User(name: String, age: Int)
来源：http://baike.sjlbkw.cn/Article/details/gduzcixbc.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.tarul.cn/Article/details/gtaijcafr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.tarul.cn/Article/details/gifhmuygp.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.vehdjk.com/Article/details/gccdwkswo.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fktsv.cn/Article/details/gukzmwqgw.sHtML

[T59] Scala：循环
来源：http://m.share.epnwcf.com/Article/details/gctkifctc.sHtML

for (i <- 1 to 10) println(i)
来源：http://blog.vehdjk.com/Article/details/gerqjeyzb.sHtML

[T60] Scala：折叠
来源：http://wap.yfazqb.com/Article/details/gqjvobpgt.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://baike.epnwcf.com/Article/details/gdszldsjs.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gkzmhndex.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.share.vehdjk.com/Article/details/ghpydjcwl.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gujdzkspn.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.vehdjk.com/Article/details/gfcbyubpt.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.tarul.cn/Article/details/glmdzpotp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://wap.tarul.cn/Article/details/gkviltxna.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.share.yfazqb.com/Article/details/getszojhc.sHtML

[U03] Py：加载 .env 配置
来源：http://read.share.yfazqb.com/Article/details/gabkpghkn.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.bbcook.cn/Article/details/glsbttyve.sHtML

[U04] Py：变量调试打印
来源：http://m.share.vehdjk.com/Article/details/gcshopgdl.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://m.share.yfazqb.com/Article/details/geuikymzh.sHtML

[U05] Py：列表去重且保序
来源：http://m.share.yfazqb.com/Article/details/gvptxayct.sHtML

list(dict.fromkeys(arr))
来源：http://www.blog.yfazqb.com/Article/details/gtsknajft.sHtML

[U06] Py：合并两个字典
来源：http://m.share.epnwcf.com/Article/details/gcwfsafzg.sHtML

{**a, **b}
来源：http://www.share.yfazqb.com/Article/details/gasysjyju.sHtML

[U07] Py：反转字典键值
来源：http://m.share.yfazqb.com/Article/details/gpmjkylfo.sHtML

{v: k for k, v in d.items()}
来源：http://www.blog.yfazqb.com/Article/details/gawftrnnv.sHtML

[U08] Py：展平二维列表
来源：http://read.share.vehdjk.com/Article/details/gjmfvqhaq.sHtML

[y for x in nested for y in x]
来源：http://baike.vehdjk.com/Article/details/gbjuqnozf.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.fktsv.cn/Article/details/gppnhhzri.sHtML

max(d, key=d.get)
来源：http://m.share.yfazqb.com/Article/details/gxuibjcyj.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.yfazqb.com/Article/details/gyzkeujcz.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.epnwcf.com/Article/details/gvseoglbw.sHtML

[U11] Py：生成器表达式
来源：http://read.share.sjlbkw.cn/Article/details/ghlhzyqyl.sHtML

(x * 2 for x in arr)
来源：http://3g.tarul.cn/Article/details/gwoxrnbge.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.epnwcf.com/Article/details/gcuaadaah.sHtML

Counter(arr).most_common(3)
来源：http://www.blog.vehdjk.com/Article/details/gbsdimkfq.sHtML

[U13] Py：固定长度队列
来源：http://www.share.yfazqb.com/Article/details/gcaqwxtoy.sHtML

deque(maxlen=10)
来源：http://read.share.tarul.cn/Article/details/gnukrcmxl.sHtML

[U14] Py：分组收集到列表
来源：http://mobile.bbcook.cn/Article/details/gqbzfjpop.sHtML

defaultdict(list)
来源：http://read.share.tarul.cn/Article/details/gddkvlwzq.sHtML

[U15] Py：高精度计时
来源：http://wap.epnwcf.com/Article/details/gyayujwhy.sHtML

t = time.perf_counter()
来源：http://www.blog.bbcook.cn/Article/details/gfyspdcnv.sHtML

[U16] Py：命令行参数解析
来源：http://www.blog.yfazqb.com/Article/details/gjyqzpyty.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mobile.sjlbkw.cn/Article/details/gxppphzso.sHtML

[U17] Py：初始化日志
来源：http://m.share.epnwcf.com/Article/details/gaxwqfvgw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.vehdjk.com/Article/details/gpfsmdjbi.sHtML

[U18] Py：预编译正则
来源：http://read.share.tarul.cn/Article/details/gjpwdwijl.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.bbcook.cn/Article/details/goccdqzmz.sHtML

[U19] Py：正则替换带回调
来源：http://baike.yfazqb.com/Article/details/gsvmedpcf.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://read.share.fktsv.cn/Article/details/gzbysowrt.sHtML

[U20] Py：缓存函数结果
来源：http://blog.sjlbkw.cn/Article/details/gzqgelust.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.vehdjk.com/Article/details/gnjbaqcvp.sHtML

[U21] Py：自定义上下文管理器
来源：http://wap.bbcook.cn/Article/details/guwctabiq.sHtML

@contextlib.contextmanager
来源：http://read.share.vehdjk.com/Article/details/guvyjqbdb.sHtML

[U22] Py：矩阵转置
来源：http://read.share.tarul.cn/Article/details/gismxujmd.sHtML

list(zip(*m))
来源：http://www.share.epnwcf.com/Article/details/gkzichqox.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.sjlbkw.cn/Article/details/gtezzbicj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.fktsv.cn/Article/details/gyyuhewjj.sHtML

[U24] Py：路径操作
来源：http://m.share.yfazqb.com/Article/details/gmesjdvsr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwcnkqmjb.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.fktsv.cn/Article/details/gvekqoawp.sHtML

csv.DictReader(f)
来源：http://wap.vehdjk.com/Article/details/gfdwzofxp.sHtML

[U26] Py：并发下载
来源：http://3g.fktsv.cn/Article/details/gkagtacxn.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.tarul.cn/Article/details/gfqteszim.sHtML

[U27] Py：异步 HTTP
来源：http://blog.fktsv.cn/Article/details/gueltrrzk.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.share.yfazqb.com/Article/details/gpamfhpxz.sHtML

[U28] Py：类型别名
来源：http://www.m.share.epnwcf.com/Article/details/gtayekfzb.sHtML

UserId = int
来源：http://www.m.share.vehdjk.com/Article/details/gayhmkgzo.sHtML

[U29] Py：属性校验
来源：http://www.m.share.epnwcf.com/Article/details/gteqvwncl.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.yfazqb.com/Article/details/gxeqbiyov.sHtML

[U30] Py：数据类
来源：http://mobile.bbcook.cn/Article/details/grzfhkhsx.sHtML

@dataclass(slots=True)
来源：http://www.share.epnwcf.com/Article/details/gvgnhrrcu.sHtML

[U31] Py：单测
来源：http://www.blog.sjlbkw.cn/Article/details/gwqjyetzc.sHtML

python -m pytest -q
来源：http://3g.fktsv.cn/Article/details/gjwznxsol.sHtML

[U32] Py：代码格式化
来源：http://blog.bbcook.cn/Article/details/guzqqvdms.sHtML

ruff format . && ruff check --fix .
来源：http://blog.sjlbkw.cn/Article/details/ghadguxio.sHtML

[U33] Py：打包发布
来源：http://baike.sjlbkw.cn/Article/details/ggcnnossn.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://blog.sjlbkw.cn/Article/details/gtgjwcolr.sHtML

[U34] Py：判断编码
来源：http://mobile.vehdjk.com/Article/details/ggxbjfpee.sHtML

chardet.detect(raw)
来源：http://mobile.bbcook.cn/Article/details/ghbeuddbs.sHtML

[U35] Py：发送邮件
来源：http://www.m.share.bbcook.cn/Article/details/gxbfspkxz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.epnwcf.com/Article/details/ggvqhiycm.sHtML

[U36] Py：定时任务
来源：http://mobile.vehdjk.com/Article/details/gwehceqek.sHtML

schedule.every(10).minutes.do(job)
来源：http://m.share.yfazqb.com/Article/details/ghpvcvnvx.sHtML

[U37] Py：读写 Excel
来源：http://3g.epnwcf.com/Article/details/gmdxoxoim.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.sjlbkw.cn/Article/details/gvacrpomb.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.sjlbkw.cn/Article/details/gmrbagbry.sHtML

Path(__file__).resolve().parent
来源：http://www.blog.bbcook.cn/Article/details/gtdoaiqcb.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.vehdjk.com/Article/details/gabdsiyky.sHtML

sys.stdout.isatty()
来源：http://www.blog.tarul.cn/Article/details/gnvyawwpu.sHtML

[U40] Py：打印到标准错误
来源：http://www.blog.bbcook.cn/Article/details/gcduobivv.sHtML

print("err", file=sys.stderr)
来源：http://baike.epnwcf.com/Article/details/ghsjbkffw.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.vehdjk.com/Article/details/gysbgkusj.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.bbcook.cn/Article/details/gjvmggoek.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.yfazqb.com/Article/details/gykyygcwd.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://blog.epnwcf.com/Article/details/gnjhowuxy.sHtML

[U43] PHP：声明命名空间
来源：http://wap.yfazqb.com/Article/details/gvcisqlsp.sHtML

namespace App\Http;
来源：http://3g.epnwcf.com/Article/details/gsfrlmjym.sHtML

[U44] PHP：开启严格类型
来源：http://blog.sjlbkw.cn/Article/details/gzswedsit.sHtML

declare(strict_types=1);
来源：http://wap.vehdjk.com/Article/details/gcomgjqyz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.vehdjk.com/Article/details/gktygypsa.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.bbcook.cn/Article/details/ggsfngbfx.sHtML

[U46] PHP：可空类型
来源：http://www.share.bbcook.cn/Article/details/gyoklauyh.sHtML

?string $name = null
来源：http://baike.vehdjk.com/Article/details/gbikgghua.sHtML

[U47] PHP：联合类型
来源：http://blog.fktsv.cn/Article/details/gjphvsrpl.sHtML

int|string $id
来源：http://www.share.yfazqb.com/Article/details/gyyfwifmn.sHtML

[U48] PHP：纯枚举
来源：http://mobile.sjlbkw.cn/Article/details/givykfhvm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.tarul.cn/Article/details/glorwnftr.sHtML

[U49] PHP：只读属性
来源：http://baike.fktsv.cn/Article/details/gmdoloari.sHtML

public readonly string $name
来源：http://www.share.yfazqb.com/Article/details/gzbullxpt.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.tarul.cn/Article/details/gtsvykzcn.sHtML

public function __construct(private int $id) {}
来源：http://m.share.vehdjk.com/Article/details/gxhdtbjhx.sHtML

[U51] PHP：数组解构
来源：http://baike.epnwcf.com/Article/details/gbtoqqdkq.sHtML

[$a, $b] = $arr;
来源：http://www.share.tarul.cn/Article/details/grqykciww.sHtML

[U52] PHP：箭头函数
来源：http://baike.fktsv.cn/Article/details/gpzwgteld.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.vehdjk.com/Article/details/gytlfnnln.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fktsv.cn/Article/details/grrpwwvjs.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.sjlbkw.cn/Article/details/gxpuqgyhb.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.tarul.cn/Article/details/gqhhhfqvd.sHtML

$obj?->method()
来源：http://www.blog.tarul.cn/Article/details/gvsqvyfwg.sHtML

[U55] PHP：match 表达式
来源：http://blog.bbcook.cn/Article/details/gnlbpuciw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.fktsv.cn/Article/details/gvmxqlxzq.sHtML

[U56] PHP：命名参数
来源：http://www.share.tarul.cn/Article/details/gbrmuugsl.sHtML

f(a: 1, b: 2)
来源：http://wap.sjlbkw.cn/Article/details/gpocvpnps.sHtML

[U57] PHP：字符串插值
来源：http://www.m.share.tarul.cn/Article/details/gihlgaucy.sHtML

"值: {$a}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gslcapjaw.sHtML

[U58] PHP：数组三件套
来源：http://blog.epnwcf.com/Article/details/gqgcevxjm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.vehdjk.com/Article/details/gidfpturn.sHtML

[U59] PHP：自定义排序
来源：http://wap.vehdjk.com/Article/details/glkaffoik.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fktsv.cn/Article/details/grwvbaoei.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fktsv.cn/Article/details/ggwmvsbic.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.sjlbkw.cn/Article/details/gyxctxzfs.sHtML

[U61] PHP：正则
来源：http://mobile.bbcook.cn/Article/details/gciirslqe.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.bbcook.cn/Article/details/gwombgaxw.sHtML

[U62] PHP：日期对象
来源：http://m.share.tarul.cn/Article/details/glgvxxfcy.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.sjlbkw.cn/Article/details/goxamodwx.sHtML

[U63] PHP：文件读写
来源：http://baike.vehdjk.com/Article/details/geacfnevy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.fktsv.cn/Article/details/gusjpyibm.sHtML

[U64] PHP：目录遍历
来源：http://www.share.bbcook.cn/Article/details/gxgjwtcig.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.fktsv.cn/Article/details/gtkqilynx.sHtML

[U65] PHP：会话
来源：http://wap.vehdjk.com/Article/details/gyyvbohhl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.sjlbkw.cn/Article/details/gzwfxyags.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fktsv.cn/Article/details/gycdkmhwq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.epnwcf.com/Article/details/guypeedqi.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.tarul.cn/Article/details/gubhfntbd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.bbcook.cn/Article/details/grqzbipgf.sHtML

[U68] PHP：PDO 连接
来源：http://baike.epnwcf.com/Article/details/gsxacxrja.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fktsv.cn/Article/details/gckmautzx.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.yfazqb.com/Article/details/ggdmmytie.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.epnwcf.com/Article/details/gjgseuiiy.sHtML

[U70] PHP：PDO 事务
来源：http://3g.tarul.cn/Article/details/gzrxhjcqm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.bbcook.cn/Article/details/gmxmqwrlr.sHtML

[U71] PHP：抛出异常
来源：http://mobile.tarul.cn/Article/details/gcerkbyfc.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fktsv.cn/Article/details/giesjcchw.sHtML

[U72] PHP：写错误日志
来源：http://www.share.epnwcf.com/Article/details/gbchjdtdb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.epnwcf.com/Article/details/gehokedos.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fktsv.cn/Article/details/gwexvrles.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.tarul.cn/Article/details/grxjtnmte.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.vehdjk.com/Article/details/ghhxqcied.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fktsv.cn/Article/details/guhaprlgy.sHtML

[U75] PHP：依赖注入
来源：http://baike.epnwcf.com/Article/details/gqwlgfdbi.sHtML

composer require psr/container
来源：http://baike.vehdjk.com/Article/details/gkjmbrjqi.sHtML

[U76] PHP：简单路由
来源：http://baike.yfazqb.com/Article/details/gdymjmsrc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.bbcook.cn/Article/details/gtbpkbhjv.sHtML

[U77] PHP：模板渲染
来源：http://mobile.vehdjk.com/Article/details/gaodfjsuw.sHtML

composer require twig/twig
来源：http://blog.vehdjk.com/Article/details/guilqgvnv.sHtML

[U78] PHP：单元测试
来源：http://3g.bbcook.cn/Article/details/gxjhcgomz.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.bbcook.cn/Article/details/goirevjka.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.vehdjk.com/Article/details/gqlnhcuok.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.yfazqb.com/Article/details/gysneerac.sHtML

[U80] PHP：代码规范修复
来源：http://wap.sjlbkw.cn/Article/details/gxfwvamzh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.yfazqb.com/Article/details/gukgkydis.sHtML

[U81] JS：初始化项目
来源：http://wap.sjlbkw.cn/Article/details/glpuenisk.sHtML

npm init -y;  npm i express
来源：http://www.m.share.sjlbkw.cn/Article/details/grcblywes.sHtML

[U82] JS：package.json 脚本
来源：http://baike.sjlbkw.cn/Article/details/gqgxadhlf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.sjlbkw.cn/Article/details/gvatmszkh.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.vehdjk.com/Article/details/gqefxtfyg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.epnwcf.com/Article/details/grluuaeuc.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.bbcook.cn/Article/details/gevjnmspz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.bbcook.cn/Article/details/gtbwamyef.sHtML

[U85] JS：可选链
来源：http://m.share.fktsv.cn/Article/details/gbeqlrmvc.sHtML

a?.b?.c
来源：http://mobile.sjlbkw.cn/Article/details/gimkxujgi.sHtML

[U86] JS：空值合并
来源：http://mobile.sjlbkw.cn/Article/details/gmrtjnvyl.sHtML

a ?? b
来源：http://www.blog.tarul.cn/Article/details/gbygqdyvf.sHtML

[U87] JS：解构默认值
来源：http://mobile.sjlbkw.cn/Article/details/gwzqhgzzq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.tarul.cn/Article/details/geqsrdsmq.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.sjlbkw.cn/Article/details/gegjgfejp.sHtML

{ ...a, ...b }
来源：http://www.blog.bbcook.cn/Article/details/gxedlzqma.sHtML

[U89] JS：数组去重
来源：http://blog.vehdjk.com/Article/details/gmkgxpalw.sHtML

[...new Set(arr)]
来源：http://3g.yfazqb.com/Article/details/gfltbdysk.sHtML

[U90] JS：数字数组排序
来源：http://blog.fktsv.cn/Article/details/gseyyrlgy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.epnwcf.com/Article/details/gfzhgoebo.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.sjlbkw.cn/Article/details/gnznkidsu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.sjlbkw.cn/Article/details/gbpauztnk.sHtML

[U92] JS：深拷贝
来源：http://blog.vehdjk.com/Article/details/gvfibkffv.sHtML

structuredClone(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gkhoevaqs.sHtML

[U93] JS：模板字符串
来源：http://m.share.bbcook.cn/Article/details/gtcjcdqrx.sHtML

`共 ${n} 条`
来源：http://baike.epnwcf.com/Article/details/gdymztcpx.sHtML

[U94] JS：箭头函数
来源：http://read.share.bbcook.cn/Article/details/glasyhpeo.sHtML

const double = x => x * 2;
来源：http://mobile.bbcook.cn/Article/details/gryfzuatj.sHtML

[U95] JS：Promise 包装
来源：http://blog.fktsv.cn/Article/details/gjxeduivu.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.yfazqb.com/Article/details/gueoztvme.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.bbcook.cn/Article/details/guwptfppz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.yfazqb.com/Article/details/ggigxjmcm.sHtML

[U97] JS：并发请求
来源：http://wap.tarul.cn/Article/details/gvwzhkigw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.tarul.cn/Article/details/gsivfervw.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.vehdjk.com/Article/details/gvdvyqsgk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.vehdjk.com/Article/details/gbgxafzae.sHtML

[U99] JS：事件监听
来源：http://read.share.yfazqb.com/Article/details/ghsksbulp.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fktsv.cn/Article/details/gflazjvpx.sHtML

[U100] JS：DOM 查询
来源：http://read.share.vehdjk.com/Article/details/gvpmkwgnp.sHtML

document.querySelector(".item")
来源：http://www.share.yfazqb.com/Article/details/gtsmhqeus.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fktsv.cn/Article/details/gkvinqmfh.sHtML

el.classList.toggle("active")
来源：http://www.blog.yfazqb.com/Article/details/gelrxavoj.sHtML

[U102] JS：本地存储
来源：http://read.share.bbcook.cn/Article/details/gqrecyizb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.yfazqb.com/Article/details/gdqmfrfms.sHtML

[U103] JS：定时器
来源：http://blog.epnwcf.com/Article/details/gqpzcmmru.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.epnwcf.com/Article/details/gbktwvnjx.sHtML

[U104] JS：防抖
来源：http://blog.tarul.cn/Article/details/gtyhgjuhl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.tarul.cn/Article/details/gmtmmsihn.sHtML

[U105] JS：节流
来源：http://mobile.vehdjk.com/Article/details/gkehyrpno.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.vehdjk.com/Article/details/gbcpsvnmo.sHtML

[U106] JS：日期格式化
来源：http://baike.sjlbkw.cn/Article/details/gdvqdprpu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.epnwcf.com/Article/details/gbbbibzyl.sHtML

[U107] JS：数字千分位
来源：http://mobile.sjlbkw.cn/Article/details/gdoqschxx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.vehdjk.com/Article/details/guvxwzscx.sHtML

[U108] JS：随机整数
来源：http://www.blog.bbcook.cn/Article/details/gnqvbbsft.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.yfazqb.com/Article/details/ggqaljuhd.sHtML

[U109] JS：数组分组
来源：http://m.share.sjlbkw.cn/Article/details/gfspcrdhn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.yfazqb.com/Article/details/gdtoqffbh.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fktsv.cn/Article/details/gudeslpck.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fktsv.cn/Article/details/gzvequiqz.sHtML

[U111] JS：对象转 Map
来源：http://wap.fktsv.cn/Article/details/glkybsipj.sHtML

new Map(Object.entries(obj))
来源：http://3g.epnwcf.com/Article/details/gyptztfkt.sHtML

[U112] JS：字符串补位
来源：http://www.blog.yfazqb.com/Article/details/gfngbdqnb.sHtML

"7".padStart(3, "0")
来源：http://3g.epnwcf.com/Article/details/grryzxhzp.sHtML

[U113] JS：正则替换全部
来源：http://mobile.sjlbkw.cn/Article/details/gkzzjkitl.sHtML

s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/gibhbhcim.sHtML

[U114] JS：JSON 深比较
来源：http://wap.yfazqb.com/Article/details/guwxnxjry.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.tarul.cn/Article/details/gohhatqfp.sHtML

[U115] JS：生成 UUID
来源：http://www.share.tarul.cn/Article/details/gsymskmyo.sHtML

crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/gfocrfaqq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.yfazqb.com/Article/details/gvpxiyvvq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.epnwcf.com/Article/details/gmdecmjot.sHtML

[U117] JS：单元测试
来源：http://blog.epnwcf.com/Article/details/gziuvakxl.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.vehdjk.com/Article/details/gdiqxvqib.sHtML

[U118] JS：开发服务器
来源：http://blog.tarul.cn/Article/details/gvraqaulk.sHtML

npm i -D vite;  npx vite
来源：http://3g.tarul.cn/Article/details/gafxiwxsg.sHtML

[U119] JS：生产构建
来源：http://mobile.epnwcf.com/Article/details/grbymewmc.sHtML

npx vite build
来源：http://baike.yfazqb.com/Article/details/gxrmrrweu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.epnwcf.com/Article/details/glokrtsku.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.sjlbkw.cn/Article/details/gsasxhnvc.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gjlnyfahk.sHtML

统计汇总
来源：http://www.blog.vehdjk.com/Article/details/gmufilvdh.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gdddzdqlf.sHtML

按语言统计（条）：
来源：http://baike.sjlbkw.cn/Article/details/gaxjstzzq.sHtML

Python ......... 252
来源：http://mobile.epnwcf.com/Article/details/gacnbqoro.sHtML

PHP ............ 252
来源：http://wap.fktsv.cn/Article/details/gogdcezcu.sHtML

JavaScript ..... 252
来源：http://read.share.fktsv.cn/Article/details/gokywhqal.sHtML

TypeScript ..... 212
来源：http://blog.epnwcf.com/Article/details/gjkimduim.sHtML

Java ........... 212
来源：http://www.blog.epnwcf.com/Article/details/gkihjwkyu.sHtML

Go ............. 212
来源：http://blog.epnwcf.com/Article/details/gtpkddbod.sHtML

Ruby ........... 212
来源：http://m.share.sjlbkw.cn/Article/details/gteayceyi.sHtML

C# ............. 212
来源：http://baike.yfazqb.com/Article/details/gteyzrljb.sHtML

C .............. 30
来源：http://baike.vehdjk.com/Article/details/gpgnjcsya.sHtML

C++ ............ 30
来源：http://m.share.bbcook.cn/Article/details/gyciecohi.sHtML

SQL ............ 90
来源：http://3g.epnwcf.com/Article/details/gvfqomcka.sHtML

Bash ........... 80
来源：http://www.blog.tarul.cn/Article/details/gwaodbpkt.sHtML

Kotlin ......... 15
来源：http://3g.tarul.cn/Article/details/gfyilqfix.sHtML

Swift .......... 15
来源：http://read.share.fktsv.cn/Article/details/gbbdirgnb.sHtML

Lua ............ 10
来源：http://www.m.share.vehdjk.com/Article/details/gbuviggxy.sHtML

Perl ........... 10
来源：http://mobile.vehdjk.com/Article/details/gqjtwqier.sHtML

Scala .......... 10
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmqpdhmp.sHtML

------------------------------------
来源：http://mobile.bbcook.cn/Article/details/gecssgrwo.sHtML

合计 ........... 2106 条
来源：http://read.share.fktsv.cn/Article/details/gmzqjenzq.sHtML

按章节统计：
来源：http://wap.yfazqb.com/Article/details/gnhxlpasp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.bbcook.cn/Article/details/gyazokfrr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.tarul.cn/Article/details/gpieealkh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.yfazqb.com/Article/details/gamidjgtu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.yfazqb.com/Article/details/gmckztkdq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.tarul.cn/Article/details/gvcvpatay.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.epnwcf.com/Article/details/gptmygpvq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.epnwcf.com/Article/details/gddrxtddw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.sjlbkw.cn/Article/details/guonxjpwo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.epnwcf.com/Article/details/gdiynwnfk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.bbcook.cn/Article/details/gjawhfoxx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.tarul.cn/Article/details/gqlqlutds.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.vehdjk.com/Article/details/gnymmuzjs.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.epnwcf.com/Article/details/gyfekqcea.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.sjlbkw.cn/Article/details/gqbnatjzf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.yfazqb.com/Article/details/grezfkatn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fktsv.cn/Article/details/ghvwzsfgi.sHtML

Q SQL 专题                              90
来源：http://www.blog.tarul.cn/Article/details/gqzelfzhj.sHtML

R Bash 专题                             80
来源：http://mobile.fktsv.cn/Article/details/gkukxjxut.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fktsv.cn/Article/details/gbwyxdcuf.sHtML

T 其他语言补充                          60
来源：http://baike.fktsv.cn/Article/details/gupirrdle.sHtML


<!-- 参考信息 -->