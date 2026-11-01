代发 wailian999

case class User(name: String, age: Int)
来源：http://blog.tarul.cn/Article/details/gstuokqui.sHtML

[T57] Scala：模式匹配
来源：http://blog.vehdjk.com/Article/details/gyywysmdc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fktsv.cn/Article/details/guxuwmybj.sHtML

[T58] Scala：函数定义
来源：http://read.share.vehdjk.com/Article/details/gyhblaxll.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.epnwcf.com/Article/details/gbnomrnhb.sHtML

[T59] Scala：循环
来源：http://baike.fktsv.cn/Article/details/giuacvhyb.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.epnwcf.com/Article/details/gaiwwvcca.sHtML

[T60] Scala：折叠
来源：http://www.blog.tarul.cn/Article/details/gzjvtmobw.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.share.tarul.cn/Article/details/gqctbfayw.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gilxeayju.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.tarul.cn/Article/details/gapdaelfh.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gnvqxazva.sHtML

[U01] Py：创建虚拟环境
来源：http://mobile.yfazqb.com/Article/details/gunxgzyfq.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.yfazqb.com/Article/details/gufiljknk.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.blog.vehdjk.com/Article/details/gcpqcywdz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.blog.tarul.cn/Article/details/gpuibzahg.sHtML

[U03] Py：加载 .env 配置
来源：http://baike.yfazqb.com/Article/details/ghrlmfeoq.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://www.m.share.vehdjk.com/Article/details/gkrqdjaxz.sHtML

[U04] Py：变量调试打印
来源：http://3g.vehdjk.com/Article/details/gzufdswkd.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://read.share.vehdjk.com/Article/details/gvpuqlqpq.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.fktsv.cn/Article/details/gshoencvc.sHtML

list(dict.fromkeys(arr))
来源：http://read.share.tarul.cn/Article/details/gvruojgsg.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.yfazqb.com/Article/details/gxnshxlpq.sHtML

{**a, **b}
来源：http://read.share.bbcook.cn/Article/details/greenephg.sHtML

[U07] Py：反转字典键值
来源：http://wap.tarul.cn/Article/details/gmapfahfw.sHtML

{v: k for k, v in d.items()}
来源：http://blog.yfazqb.com/Article/details/gvsaovsmm.sHtML

[U08] Py：展平二维列表
来源：http://m.share.epnwcf.com/Article/details/gghvlvwbw.sHtML

[y for x in nested for y in x]
来源：http://www.blog.bbcook.cn/Article/details/ghaudwdfr.sHtML

[U09] Py：字典取最大值的键
来源：http://m.share.epnwcf.com/Article/details/gvldkivsj.sHtML

max(d, key=d.get)
来源：http://m.share.epnwcf.com/Article/details/gadmbnoia.sHtML

[U10] Py：按值排序字典
来源：http://www.m.share.epnwcf.com/Article/details/gjaczcgne.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://m.share.bbcook.cn/Article/details/gzqvwbkxk.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fktsv.cn/Article/details/gshijexpe.sHtML

(x * 2 for x in arr)
来源：http://baike.bbcook.cn/Article/details/gfaipiqcj.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.vehdjk.com/Article/details/gtgfmbsxt.sHtML

Counter(arr).most_common(3)
来源：http://read.share.tarul.cn/Article/details/gmesigddu.sHtML

[U13] Py：固定长度队列
来源：http://mobile.yfazqb.com/Article/details/gdnflzyta.sHtML

deque(maxlen=10)
来源：http://mobile.vehdjk.com/Article/details/gioaoyxza.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.vehdjk.com/Article/details/gwymlyrsl.sHtML

defaultdict(list)
来源：http://3g.tarul.cn/Article/details/gnisaonad.sHtML

[U15] Py：高精度计时
来源：http://blog.tarul.cn/Article/details/gdyzpnclf.sHtML

t = time.perf_counter()
来源：http://wap.epnwcf.com/Article/details/gadinayvn.sHtML

[U16] Py：命令行参数解析
来源：http://m.share.vehdjk.com/Article/details/gmfyzelhl.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.bbcook.cn/Article/details/gdlhpozoh.sHtML

[U17] Py：初始化日志
来源：http://mobile.sjlbkw.cn/Article/details/gtozcyyov.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.epnwcf.com/Article/details/gzsgvhcqr.sHtML

[U18] Py：预编译正则
来源：http://blog.tarul.cn/Article/details/gojznctmv.sHtML

pat = re.compile(r"\d+")
来源：http://blog.tarul.cn/Article/details/ggcvsazir.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.sjlbkw.cn/Article/details/gkvksemog.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.yfazqb.com/Article/details/ggalkbtel.sHtML

[U20] Py：缓存函数结果
来源：http://wap.yfazqb.com/Article/details/grdelptyg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.epnwcf.com/Article/details/gohqrdzcs.sHtML

[U21] Py：自定义上下文管理器
来源：http://read.share.vehdjk.com/Article/details/gmpenssjx.sHtML

@contextlib.contextmanager
来源：http://blog.tarul.cn/Article/details/gccxhqkyo.sHtML

[U22] Py：矩阵转置
来源：http://blog.yfazqb.com/Article/details/gpprprjhx.sHtML

list(zip(*m))
来源：http://mobile.tarul.cn/Article/details/gvoowjets.sHtML

[U23] Py：分块读取大文件
来源：http://www.share.epnwcf.com/Article/details/grmrnanzk.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.sjlbkw.cn/Article/details/gvjzmdzee.sHtML

[U24] Py：路径操作
来源：http://www.share.fktsv.cn/Article/details/gzakiehpd.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.epnwcf.com/Article/details/gpknrbpbr.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fktsv.cn/Article/details/grukoatsh.sHtML

csv.DictReader(f)
来源：http://read.share.epnwcf.com/Article/details/ggwhfqzcb.sHtML

[U26] Py：并发下载
来源：http://mobile.vehdjk.com/Article/details/gsmvttfcq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://3g.sjlbkw.cn/Article/details/gkcpojlmg.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.yfazqb.com/Article/details/gifaukdnt.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.m.share.vehdjk.com/Article/details/gznpueaob.sHtML

[U28] Py：类型别名
来源：http://www.share.fktsv.cn/Article/details/grxqwbxxs.sHtML

UserId = int
来源：http://read.share.yfazqb.com/Article/details/gfsycurxt.sHtML

[U29] Py：属性校验
来源：http://mobile.vehdjk.com/Article/details/gohrdbicy.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.epnwcf.com/Article/details/gsbaovsjx.sHtML

[U30] Py：数据类
来源：http://m.share.epnwcf.com/Article/details/gkodaqwgi.sHtML

@dataclass(slots=True)
来源：http://wap.vehdjk.com/Article/details/gsaqbxghp.sHtML

[U31] Py：单测
来源：http://3g.fktsv.cn/Article/details/gtqycywvn.sHtML

python -m pytest -q
来源：http://m.share.fktsv.cn/Article/details/gunoioagv.sHtML

[U32] Py：代码格式化
来源：http://wap.yfazqb.com/Article/details/gmtrkedoc.sHtML

ruff format . && ruff check --fix .
来源：http://www.blog.tarul.cn/Article/details/gdqbwedlj.sHtML

[U33] Py：打包发布
来源：http://3g.epnwcf.com/Article/details/gnibatmri.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.m.share.bbcook.cn/Article/details/gwblzifah.sHtML

[U34] Py：判断编码
来源：http://3g.sjlbkw.cn/Article/details/gfmbfhftk.sHtML

chardet.detect(raw)
来源：http://www.m.share.vehdjk.com/Article/details/gjyoxadhn.sHtML

[U35] Py：发送邮件
来源：http://mobile.tarul.cn/Article/details/gadilfgrq.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.m.share.yfazqb.com/Article/details/gqzhipucu.sHtML

[U36] Py：定时任务
来源：http://www.blog.bbcook.cn/Article/details/gxcbfcabv.sHtML

schedule.every(10).minutes.do(job)
来源：http://wap.vehdjk.com/Article/details/gahqkspgl.sHtML

[U37] Py：读写 Excel
来源：http://mobile.bbcook.cn/Article/details/gwuqkcpdh.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.share.sjlbkw.cn/Article/details/gexcfaamh.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.vehdjk.com/Article/details/gcskdddrj.sHtML

Path(__file__).resolve().parent
来源：http://read.share.tarul.cn/Article/details/gsowbjfjo.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.sjlbkw.cn/Article/details/gulegfwwu.sHtML

sys.stdout.isatty()
来源：http://baike.fktsv.cn/Article/details/gttxvdftm.sHtML

[U40] Py：打印到标准错误
来源：http://blog.fktsv.cn/Article/details/gunzglkjl.sHtML

print("err", file=sys.stderr)
来源：http://blog.sjlbkw.cn/Article/details/gucuvityi.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.fktsv.cn/Article/details/ghgwawkne.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.tarul.cn/Article/details/gixblubvr.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.bbcook.cn/Article/details/gktabtmuc.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.vehdjk.com/Article/details/gjesfcktv.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.vehdjk.com/Article/details/gnjbmcvlm.sHtML

namespace App\Http;
来源：http://www.m.share.bbcook.cn/Article/details/gvltatpql.sHtML

[U44] PHP：开启严格类型
来源：http://baike.sjlbkw.cn/Article/details/ghcsobfxe.sHtML

declare(strict_types=1);
来源：http://baike.fktsv.cn/Article/details/giwdeqdie.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fktsv.cn/Article/details/gyocopoyj.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.epnwcf.com/Article/details/gxgprzidm.sHtML

[U46] PHP：可空类型
来源：http://baike.sjlbkw.cn/Article/details/gojxcwezr.sHtML

?string $name = null
来源：http://baike.bbcook.cn/Article/details/gnletprfz.sHtML

[U47] PHP：联合类型
来源：http://3g.yfazqb.com/Article/details/gidwgalyw.sHtML

int|string $id
来源：http://3g.yfazqb.com/Article/details/gscmsunvy.sHtML

[U48] PHP：纯枚举
来源：http://m.share.fktsv.cn/Article/details/gdhbrcqdd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.bbcook.cn/Article/details/gdztalhte.sHtML

[U49] PHP：只读属性
来源：http://mobile.fktsv.cn/Article/details/goohjkyjx.sHtML

public readonly string $name
来源：http://mobile.vehdjk.com/Article/details/giriijnln.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.fktsv.cn/Article/details/gysjgizvj.sHtML

public function __construct(private int $id) {}
来源：http://baike.bbcook.cn/Article/details/gwxpssmbb.sHtML

[U51] PHP：数组解构
来源：http://www.blog.sjlbkw.cn/Article/details/gothbcvhw.sHtML

[$a, $b] = $arr;
来源：http://read.share.bbcook.cn/Article/details/ghluwxzde.sHtML

[U52] PHP：箭头函数
来源：http://baike.sjlbkw.cn/Article/details/gqcthqkdp.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.bbcook.cn/Article/details/gcenkmutx.sHtML

[U53] PHP：空合并运算符
来源：http://wap.yfazqb.com/Article/details/gjvmewwrr.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.epnwcf.com/Article/details/gmfcsbwsb.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.epnwcf.com/Article/details/ggirbyrbs.sHtML

$obj?->method()
来源：http://blog.bbcook.cn/Article/details/gwetprvod.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fktsv.cn/Article/details/gveccrnxs.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.fktsv.cn/Article/details/gmigcgayt.sHtML

[U56] PHP：命名参数
来源：http://mobile.epnwcf.com/Article/details/gdiimrrtn.sHtML

f(a: 1, b: 2)
来源：http://read.share.fktsv.cn/Article/details/ggpneclxw.sHtML

[U57] PHP：字符串插值
来源：http://www.share.epnwcf.com/Article/details/gvyzlgdyb.sHtML

"值: {$a}"
来源：http://www.blog.bbcook.cn/Article/details/gayokdnns.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fktsv.cn/Article/details/gkrxndsyu.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.epnwcf.com/Article/details/ginooyssh.sHtML

[U59] PHP：自定义排序
来源：http://3g.bbcook.cn/Article/details/gjjpjwwop.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.epnwcf.com/Article/details/gylhebeig.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fktsv.cn/Article/details/gqrxvqtsh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.epnwcf.com/Article/details/gdisrhwlr.sHtML

[U61] PHP：正则
来源：http://mobile.tarul.cn/Article/details/gmgovbpgj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.epnwcf.com/Article/details/ggulpatee.sHtML

[U62] PHP：日期对象
来源：http://wap.tarul.cn/Article/details/geuibxrmw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.tarul.cn/Article/details/gpcegwoyc.sHtML

[U63] PHP：文件读写
来源：http://mobile.epnwcf.com/Article/details/grmbqnvly.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fktsv.cn/Article/details/gnosefhfk.sHtML

[U64] PHP：目录遍历
来源：http://3g.fktsv.cn/Article/details/goknvdgcl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.fktsv.cn/Article/details/gyxtyylxw.sHtML

[U65] PHP：会话
来源：http://www.blog.vehdjk.com/Article/details/gybuauxra.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fktsv.cn/Article/details/gszpylrvc.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.epnwcf.com/Article/details/gzqcbxfov.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.tarul.cn/Article/details/geiaeuoog.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.yfazqb.com/Article/details/giwksbdsg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.yfazqb.com/Article/details/glyppkkbc.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.yfazqb.com/Article/details/gmqudwomw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.sjlbkw.cn/Article/details/ghxsgmmxa.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.fktsv.cn/Article/details/gkykrtnif.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.tarul.cn/Article/details/ghlzuwfry.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.tarul.cn/Article/details/gqbufsdjv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.sjlbkw.cn/Article/details/gtoomtuaz.sHtML

[U71] PHP：抛出异常
来源：http://baike.tarul.cn/Article/details/gosesypdf.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.epnwcf.com/Article/details/gssvnvqic.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.tarul.cn/Article/details/gdcxaecpq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.epnwcf.com/Article/details/gbweaeyay.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.fktsv.cn/Article/details/gxhvjkaqa.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.bbcook.cn/Article/details/gxkxtgnni.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.sjlbkw.cn/Article/details/gltvvgtwa.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.epnwcf.com/Article/details/gizygpqmt.sHtML

[U75] PHP：依赖注入
来源：http://www.share.epnwcf.com/Article/details/gfmouoood.sHtML

composer require psr/container
来源：http://www.m.share.yfazqb.com/Article/details/gfetrqxwk.sHtML

[U76] PHP：简单路由
来源：http://www.share.fktsv.cn/Article/details/gynbmvigk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fktsv.cn/Article/details/ggcxsowzv.sHtML

[U77] PHP：模板渲染
来源：http://wap.fktsv.cn/Article/details/gzqcgwlws.sHtML

composer require twig/twig
来源：http://read.share.bbcook.cn/Article/details/gwmctxwue.sHtML

[U78] PHP：单元测试
来源：http://blog.bbcook.cn/Article/details/gjyrlqoni.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.vehdjk.com/Article/details/gkokixaxt.sHtML

[U79] PHP：静态分析
来源：http://www.share.sjlbkw.cn/Article/details/gmmxiarot.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.epnwcf.com/Article/details/gaqibbhvr.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.vehdjk.com/Article/details/grdkyftcf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.tarul.cn/Article/details/gksbuqwtj.sHtML

[U81] JS：初始化项目
来源：http://www.blog.yfazqb.com/Article/details/gcujxzgta.sHtML

npm init -y;  npm i express
来源：http://mobile.fktsv.cn/Article/details/gmclbtbov.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.bbcook.cn/Article/details/ggvbkgszo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.epnwcf.com/Article/details/gxwfehfog.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.vehdjk.com/Article/details/gufeselhx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.sjlbkw.cn/Article/details/grhkmxnnn.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.epnwcf.com/Article/details/gcrtwigdw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fktsv.cn/Article/details/gkiakdxzf.sHtML

[U85] JS：可选链
来源：http://wap.fktsv.cn/Article/details/gzcgorayi.sHtML

a?.b?.c
来源：http://m.share.bbcook.cn/Article/details/gytgibgcz.sHtML

[U86] JS：空值合并
来源：http://baike.sjlbkw.cn/Article/details/gyiparzrq.sHtML

a ?? b
来源：http://m.share.epnwcf.com/Article/details/gbwcmzoro.sHtML

[U87] JS：解构默认值
来源：http://www.blog.vehdjk.com/Article/details/gazmqxamg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.tarul.cn/Article/details/ghzkfysvl.sHtML

[U88] JS：对象展开合并
来源：http://wap.sjlbkw.cn/Article/details/gwlgdqjer.sHtML

{ ...a, ...b }
来源：http://baike.tarul.cn/Article/details/gahvfpjkx.sHtML

[U89] JS：数组去重
来源：http://read.share.vehdjk.com/Article/details/gynbylccc.sHtML

[...new Set(arr)]
来源：http://wap.epnwcf.com/Article/details/gxyccvdnm.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.yfazqb.com/Article/details/gdktxgyrw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/gzelsgmdm.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fktsv.cn/Article/details/gwziawnew.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.tarul.cn/Article/details/guhfkhimz.sHtML

[U92] JS：深拷贝
来源：http://mobile.vehdjk.com/Article/details/gakxmsluz.sHtML

structuredClone(obj)
来源：http://read.share.bbcook.cn/Article/details/gbsjuzzzx.sHtML

[U93] JS：模板字符串
来源：http://baike.tarul.cn/Article/details/gejaioscv.sHtML

`共 ${n} 条`
来源：http://wap.fktsv.cn/Article/details/gxrcmuesd.sHtML

[U94] JS：箭头函数
来源：http://m.share.sjlbkw.cn/Article/details/gliygzwrg.sHtML

const double = x => x * 2;
来源：http://wap.tarul.cn/Article/details/gboqelxrv.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.vehdjk.com/Article/details/gwcosnitd.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.yfazqb.com/Article/details/gvqrieuzg.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfmknygr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.yfazqb.com/Article/details/gmxbokmcb.sHtML

[U97] JS：并发请求
来源：http://www.blog.bbcook.cn/Article/details/gafvyvmab.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.bbcook.cn/Article/details/gbhuvveys.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.sjlbkw.cn/Article/details/gmbvinotb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.vehdjk.com/Article/details/gratibimn.sHtML

[U99] JS：事件监听
来源：http://blog.bbcook.cn/Article/details/gzpqsusbg.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.sjlbkw.cn/Article/details/grlriztmu.sHtML

[U100] JS：DOM 查询
来源：http://3g.yfazqb.com/Article/details/ggieohfqh.sHtML

document.querySelector(".item")
来源：http://mobile.bbcook.cn/Article/details/gduvxekze.sHtML

[U101] JS：classList 操作
来源：http://mobile.bbcook.cn/Article/details/gxjvsvyyv.sHtML

el.classList.toggle("active")
来源：http://mobile.vehdjk.com/Article/details/gaiaovxbq.sHtML

[U102] JS：本地存储
来源：http://baike.epnwcf.com/Article/details/gskvlumnn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.bbcook.cn/Article/details/gktesaaju.sHtML

[U103] JS：定时器
来源：http://read.share.sjlbkw.cn/Article/details/gxwwaosyw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmsdiwkw.sHtML

[U104] JS：防抖
来源：http://www.blog.bbcook.cn/Article/details/gpbrajqgy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.sjlbkw.cn/Article/details/gnqbsufxl.sHtML

[U105] JS：节流
来源：http://baike.sjlbkw.cn/Article/details/gnbsskowb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.vehdjk.com/Article/details/gewgczohp.sHtML

[U106] JS：日期格式化
来源：http://baike.fktsv.cn/Article/details/gtvadicrz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.epnwcf.com/Article/details/gyhrfhgfp.sHtML

[U107] JS：数字千分位
来源：http://www.blog.epnwcf.com/Article/details/gssujvlvk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.fktsv.cn/Article/details/gzfadciem.sHtML

[U108] JS：随机整数
来源：http://3g.tarul.cn/Article/details/gmpvmtjnd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.epnwcf.com/Article/details/gmucsjuhc.sHtML

[U109] JS：数组分组
来源：http://mobile.yfazqb.com/Article/details/gjtndyigj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.epnwcf.com/Article/details/gyqdgswfx.sHtML

[U110] JS：数组分块
来源：http://www.share.tarul.cn/Article/details/gwssriegq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.vehdjk.com/Article/details/gpbaibwae.sHtML

[U111] JS：对象转 Map
来源：http://blog.fktsv.cn/Article/details/gbqmexupb.sHtML

new Map(Object.entries(obj))
来源：http://wap.vehdjk.com/Article/details/gzbjgvgnc.sHtML

[U112] JS：字符串补位
来源：http://m.share.sjlbkw.cn/Article/details/gagdbgeau.sHtML

"7".padStart(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/guiiwuewq.sHtML

[U113] JS：正则替换全部
来源：http://baike.bbcook.cn/Article/details/glbkxdbuf.sHtML

s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/gpdkspbpl.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.vehdjk.com/Article/details/gmobbkzfe.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fktsv.cn/Article/details/ggowmatfv.sHtML

[U115] JS：生成 UUID
来源：http://www.share.vehdjk.com/Article/details/gqmnqrxgd.sHtML

crypto.randomUUID()
来源：http://3g.yfazqb.com/Article/details/garlnvkps.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.vehdjk.com/Article/details/gwnwuhbal.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.sjlbkw.cn/Article/details/gekmipjcl.sHtML

[U117] JS：单元测试
来源：http://wap.fktsv.cn/Article/details/glrzhhsuu.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.tarul.cn/Article/details/gkihpkwkw.sHtML

[U118] JS：开发服务器
来源：http://wap.fktsv.cn/Article/details/gobaxtjqk.sHtML

npm i -D vite;  npx vite
来源：http://m.share.vehdjk.com/Article/details/gxxwsghco.sHtML

[U119] JS：生产构建
来源：http://www.m.share.vehdjk.com/Article/details/gccdqqwhb.sHtML

npx vite build
来源：http://www.share.epnwcf.com/Article/details/ggjgtoqgx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.sjlbkw.cn/Article/details/gfmkzqsrg.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.tarul.cn/Article/details/gwzcjreuo.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gkkhbgtkh.sHtML

统计汇总
来源：http://baike.sjlbkw.cn/Article/details/ghivrsjkp.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/ghxpuvlem.sHtML

按语言统计（条）：
来源：http://blog.epnwcf.com/Article/details/guwxcsanl.sHtML

Python ......... 252
来源：http://m.share.sjlbkw.cn/Article/details/gjlutvady.sHtML

PHP ............ 252
来源：http://www.share.epnwcf.com/Article/details/gclokfbgv.sHtML

JavaScript ..... 252
来源：http://wap.epnwcf.com/Article/details/gqpdpjrqk.sHtML

TypeScript ..... 212
来源：http://baike.fktsv.cn/Article/details/gfptyksis.sHtML

Java ........... 212
来源：http://www.share.fktsv.cn/Article/details/guzinrbqn.sHtML

Go ............. 212
来源：http://wap.yfazqb.com/Article/details/gwpvqcare.sHtML

Ruby ........... 212
来源：http://read.share.vehdjk.com/Article/details/gcdjisvcw.sHtML

C# ............. 212
来源：http://blog.yfazqb.com/Article/details/ggcvzkvjy.sHtML

C .............. 30
来源：http://m.share.fktsv.cn/Article/details/gzoakctzd.sHtML

C++ ............ 30
来源：http://m.share.sjlbkw.cn/Article/details/ghazqasow.sHtML

SQL ............ 90
来源：http://blog.epnwcf.com/Article/details/gwmflzxrs.sHtML

Bash ........... 80
来源：http://blog.epnwcf.com/Article/details/gsylqunnn.sHtML

Kotlin ......... 15
来源：http://m.share.vehdjk.com/Article/details/giagbruri.sHtML

Swift .......... 15
来源：http://3g.fktsv.cn/Article/details/ghhirorbm.sHtML

Lua ............ 10
来源：http://wap.vehdjk.com/Article/details/goqdoazzw.sHtML

Perl ........... 10
来源：http://mobile.yfazqb.com/Article/details/gawemmzxg.sHtML

Scala .......... 10
来源：http://3g.epnwcf.com/Article/details/gljsunoxr.sHtML

------------------------------------
来源：http://www.share.sjlbkw.cn/Article/details/gwmuzazcy.sHtML

合计 ........... 2106 条
来源：http://www.blog.yfazqb.com/Article/details/gfnrzmmne.sHtML

按章节统计：
来源：http://www.share.bbcook.cn/Article/details/ghmhbucwz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.epnwcf.com/Article/details/gybhmpwjx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.tarul.cn/Article/details/gppjdmuwo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fktsv.cn/Article/details/gnzblkeau.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.bbcook.cn/Article/details/gbugfrjnp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.yfazqb.com/Article/details/ghzspcnub.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.bbcook.cn/Article/details/gurqsolnl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.bbcook.cn/Article/details/geapwcyfg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.bbcook.cn/Article/details/gexhtcxld.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gdrmaydkc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.epnwcf.com/Article/details/gpccsnnxg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/gvunoeiin.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.yfazqb.com/Article/details/ggkbdvyym.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.epnwcf.com/Article/details/glsrnebjx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.tarul.cn/Article/details/gayazazjk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.vehdjk.com/Article/details/gyomagwgg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.epnwcf.com/Article/details/galwmphou.sHtML

Q SQL 专题                              90
来源：http://3g.yfazqb.com/Article/details/gyejgznuh.sHtML

R Bash 专题                             80
来源：http://www.blog.yfazqb.com/Article/details/geiexddby.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.sjlbkw.cn/Article/details/geyxcuclb.sHtML

T 其他语言补充                          60
来源：http://read.share.sjlbkw.cn/Article/details/ggzzvyoba.sHtML

U 高频实用片段                         120
来源：http://www.blog.vehdjk.com/Article/details/gydibfqvb.sHtML

------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gmmdqogyo.sHtML

合计                                  2106 条
来源：http://m.share.epnwcf.com/Article/details/gkqdqulrv.sHtML

--------------------------------------------------------------------------------
来源：http://baike.epnwcf.com/Article/details/gtamgpfkg.sHtML


<!-- 参考信息 -->