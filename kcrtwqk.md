代发 wailian999

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fktsv.cn/Article/details/gzwrxophb.sHtML

[T59] Scala：循环
来源：http://blog.sjlbkw.cn/Article/details/gebrsiivu.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.epnwcf.com/Article/details/gjejzllcc.sHtML

[T60] Scala：折叠
来源：http://3g.tarul.cn/Article/details/gztkypaeu.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.sjlbkw.cn/Article/details/gdmbovjcm.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/guhmabtxj.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mobile.bbcook.cn/Article/details/gpugyupmx.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gyjczorvk.sHtML

[U01] Py：创建虚拟环境
来源：http://3g.sjlbkw.cn/Article/details/gdmfwzhmu.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.blog.sjlbkw.cn/Article/details/gotevuzdf.sHtML

[U02] Py：导出 / 安装依赖
来源：http://blog.epnwcf.com/Article/details/guslmfdgz.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.m.share.fktsv.cn/Article/details/gngagyqhi.sHtML

[U03] Py：加载 .env 配置
来源：http://www.share.epnwcf.com/Article/details/ggytgmslx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://baike.tarul.cn/Article/details/gcahcxzcd.sHtML

[U04] Py：变量调试打印
来源：http://m.share.yfazqb.com/Article/details/gojxsvozw.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wap.bbcook.cn/Article/details/gqtevsmoo.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.yfazqb.com/Article/details/gfjsxmlol.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.bbcook.cn/Article/details/guyglhqxt.sHtML

[U06] Py：合并两个字典
来源：http://mobile.tarul.cn/Article/details/gksuorxjf.sHtML

{**a, **b}
来源：http://m.share.yfazqb.com/Article/details/gzmleeuop.sHtML

[U07] Py：反转字典键值
来源：http://blog.sjlbkw.cn/Article/details/gghxsjamx.sHtML

{v: k for k, v in d.items()}
来源：http://3g.epnwcf.com/Article/details/gsedouuxq.sHtML

[U08] Py：展平二维列表
来源：http://www.m.share.tarul.cn/Article/details/grboelfvv.sHtML

[y for x in nested for y in x]
来源：http://www.blog.yfazqb.com/Article/details/gweaxbavj.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.vehdjk.com/Article/details/glcxkeela.sHtML

max(d, key=d.get)
来源：http://blog.fktsv.cn/Article/details/gexygbcwh.sHtML

[U10] Py：按值排序字典
来源：http://wap.sjlbkw.cn/Article/details/gidyziocm.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.sjlbkw.cn/Article/details/gvlaeohvs.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.fktsv.cn/Article/details/gvuldxexr.sHtML

(x * 2 for x in arr)
来源：http://3g.tarul.cn/Article/details/gdtelqfqi.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.tarul.cn/Article/details/gegqobkpo.sHtML

Counter(arr).most_common(3)
来源：http://mobile.yfazqb.com/Article/details/gwjvrmqno.sHtML

[U13] Py：固定长度队列
来源：http://www.share.epnwcf.com/Article/details/glcpjdsjd.sHtML

deque(maxlen=10)
来源：http://www.m.share.yfazqb.com/Article/details/gdaqzmetr.sHtML

[U14] Py：分组收集到列表
来源：http://www.blog.epnwcf.com/Article/details/gqrxngoii.sHtML

defaultdict(list)
来源：http://www.blog.vehdjk.com/Article/details/gkpifxptr.sHtML

[U15] Py：高精度计时
来源：http://mobile.sjlbkw.cn/Article/details/guyxjxscj.sHtML

t = time.perf_counter()
来源：http://www.share.fktsv.cn/Article/details/gohoqwcff.sHtML

[U16] Py：命令行参数解析
来源：http://www.share.sjlbkw.cn/Article/details/gyqwypxce.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.tarul.cn/Article/details/gzpjqxwee.sHtML

[U17] Py：初始化日志
来源：http://m.share.yfazqb.com/Article/details/ggiekdwvi.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.bbcook.cn/Article/details/gzwwvtptq.sHtML

[U18] Py：预编译正则
来源：http://www.share.vehdjk.com/Article/details/gmcdznolo.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.epnwcf.com/Article/details/gpzeazzut.sHtML

[U19] Py：正则替换带回调
来源：http://m.share.epnwcf.com/Article/details/ghzxkhixl.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.m.share.vehdjk.com/Article/details/gbevmuyyk.sHtML

[U20] Py：缓存函数结果
来源：http://mobile.bbcook.cn/Article/details/gzbhgumwm.sHtML

@functools.lru_cache(maxsize=None)
来源：http://baike.yfazqb.com/Article/details/gmrxofzja.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.share.bbcook.cn/Article/details/gehafwgsl.sHtML

@contextlib.contextmanager
来源：http://www.blog.fktsv.cn/Article/details/gkuefzxzv.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.tarul.cn/Article/details/gjepfeciq.sHtML

list(zip(*m))
来源：http://www.blog.epnwcf.com/Article/details/gpufgzbdi.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.yfazqb.com/Article/details/gaengalxf.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wap.bbcook.cn/Article/details/gncitqvoe.sHtML

[U24] Py：路径操作
来源：http://baike.sjlbkw.cn/Article/details/grmkvgrms.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://3g.tarul.cn/Article/details/gmelbkrjp.sHtML

[U25] Py：CSV 按字典读
来源：http://www.m.share.fktsv.cn/Article/details/gqaefttsj.sHtML

csv.DictReader(f)
来源：http://www.share.sjlbkw.cn/Article/details/gsoqjllwe.sHtML

[U26] Py：并发下载
来源：http://read.share.vehdjk.com/Article/details/glupursja.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://blog.fktsv.cn/Article/details/goshejvry.sHtML

[U27] Py：异步 HTTP
来源：http://baike.fktsv.cn/Article/details/guxlnmlku.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://m.share.tarul.cn/Article/details/glajdfjvp.sHtML

[U28] Py：类型别名
来源：http://www.share.epnwcf.com/Article/details/gxkzecvmb.sHtML

UserId = int
来源：http://www.share.epnwcf.com/Article/details/gzxlxaxwy.sHtML

[U29] Py：属性校验
来源：http://mobile.vehdjk.com/Article/details/ggiidzaov.sHtML

@property 与 @x.setter 配合
来源：http://read.share.tarul.cn/Article/details/ghzqoltww.sHtML

[U30] Py：数据类
来源：http://mobile.sjlbkw.cn/Article/details/gaatnpuis.sHtML

@dataclass(slots=True)
来源：http://www.m.share.tarul.cn/Article/details/gxzynzxnz.sHtML

[U31] Py：单测
来源：http://3g.tarul.cn/Article/details/grsthusao.sHtML

python -m pytest -q
来源：http://3g.sjlbkw.cn/Article/details/gmaqmubqg.sHtML

[U32] Py：代码格式化
来源：http://www.share.vehdjk.com/Article/details/grlintrlt.sHtML

ruff format . && ruff check --fix .
来源：http://www.share.fktsv.cn/Article/details/gwqclpysj.sHtML

[U33] Py：打包发布
来源：http://blog.vehdjk.com/Article/details/gixeugial.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.yfazqb.com/Article/details/gbxguufob.sHtML

[U34] Py：判断编码
来源：http://mobile.epnwcf.com/Article/details/gbaiujipk.sHtML

chardet.detect(raw)
来源：http://baike.yfazqb.com/Article/details/gkdvaglxi.sHtML

[U35] Py：发送邮件
来源：http://3g.bbcook.cn/Article/details/gjglxusra.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://blog.fktsv.cn/Article/details/gkagcswvs.sHtML

[U36] Py：定时任务
来源：http://wap.yfazqb.com/Article/details/geiutpjhe.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.bbcook.cn/Article/details/gejhszcby.sHtML

[U37] Py：读写 Excel
来源：http://baike.yfazqb.com/Article/details/gqtopzshd.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.tarul.cn/Article/details/ghpsfshpe.sHtML

[U38] Py：获取脚本所在目录
来源：http://blog.fktsv.cn/Article/details/gefmcdpqv.sHtML

Path(__file__).resolve().parent
来源：http://wap.vehdjk.com/Article/details/ggfugpazt.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.yfazqb.com/Article/details/gxixfybvg.sHtML

sys.stdout.isatty()
来源：http://baike.vehdjk.com/Article/details/gjxzavkjg.sHtML

[U40] Py：打印到标准错误
来源：http://baike.bbcook.cn/Article/details/grrrwrunv.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.fktsv.cn/Article/details/galkfhzax.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fktsv.cn/Article/details/gxtsfuskr.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.tarul.cn/Article/details/goemumgzl.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.epnwcf.com/Article/details/gssqdgsua.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.blog.tarul.cn/Article/details/gsgpkjfij.sHtML

[U43] PHP：声明命名空间
来源：http://www.blog.fktsv.cn/Article/details/grvleeoum.sHtML

namespace App\Http;
来源：http://www.m.share.fktsv.cn/Article/details/gmhnfascv.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.fktsv.cn/Article/details/gkoixifcp.sHtML

declare(strict_types=1);
来源：http://read.share.fktsv.cn/Article/details/ghnnmscep.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.blog.tarul.cn/Article/details/gujvenuoa.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.sjlbkw.cn/Article/details/ggmggpqyp.sHtML

[U46] PHP：可空类型
来源：http://blog.bbcook.cn/Article/details/giqnfhimw.sHtML

?string $name = null
来源：http://wap.fktsv.cn/Article/details/gfhjzgyhb.sHtML

[U47] PHP：联合类型
来源：http://3g.sjlbkw.cn/Article/details/gtsruxgbk.sHtML

int|string $id
来源：http://www.m.share.tarul.cn/Article/details/gitdzpfea.sHtML

[U48] PHP：纯枚举
来源：http://mobile.fktsv.cn/Article/details/gxorperei.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.yfazqb.com/Article/details/gzjkvbahn.sHtML

[U49] PHP：只读属性
来源：http://wap.vehdjk.com/Article/details/gptmochaq.sHtML

public readonly string $name
来源：http://www.share.sjlbkw.cn/Article/details/gqpnowrhf.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.sjlbkw.cn/Article/details/ghypejxmw.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.bbcook.cn/Article/details/geebyuila.sHtML

[U51] PHP：数组解构
来源：http://wap.fktsv.cn/Article/details/gwprfnvxf.sHtML

[$a, $b] = $arr;
来源：http://blog.fktsv.cn/Article/details/gvmpbovnz.sHtML

[U52] PHP：箭头函数
来源：http://3g.yfazqb.com/Article/details/goeedeytu.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.vehdjk.com/Article/details/ghxvmcbzj.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.vehdjk.com/Article/details/gzmylkxhm.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.vehdjk.com/Article/details/gnilawzya.sHtML

[U54] PHP：空安全调用
来源：http://read.share.epnwcf.com/Article/details/gzwjmgcfw.sHtML

$obj?->method()
来源：http://baike.bbcook.cn/Article/details/gujkotiee.sHtML

[U55] PHP：match 表达式
来源：http://3g.tarul.cn/Article/details/gknihjxrf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.bbcook.cn/Article/details/ghrwvgnqc.sHtML

[U56] PHP：命名参数
来源：http://blog.sjlbkw.cn/Article/details/gwibrtxoa.sHtML

f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gyhcwhcji.sHtML

[U57] PHP：字符串插值
来源：http://blog.fktsv.cn/Article/details/gprknhell.sHtML

"值: {$a}"
来源：http://wap.yfazqb.com/Article/details/guytpvrpb.sHtML

[U58] PHP：数组三件套
来源：http://blog.sjlbkw.cn/Article/details/grdgzydhm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.yfazqb.com/Article/details/gqgllbmlp.sHtML

[U59] PHP：自定义排序
来源：http://wap.sjlbkw.cn/Article/details/gvqhteznq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.sjlbkw.cn/Article/details/gpdpmiwvw.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fktsv.cn/Article/details/gxrpaixwg.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.vehdjk.com/Article/details/gnxnzamcy.sHtML

[U61] PHP：正则
来源：http://www.m.share.vehdjk.com/Article/details/gdqxrrwdl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.vehdjk.com/Article/details/ggeegwzpy.sHtML

[U62] PHP：日期对象
来源：http://www.blog.tarul.cn/Article/details/gthcgfonm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.epnwcf.com/Article/details/glbwljvyc.sHtML

[U63] PHP：文件读写
来源：http://m.share.yfazqb.com/Article/details/ghgheyeds.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.vehdjk.com/Article/details/gcimnefyt.sHtML

[U64] PHP：目录遍历
来源：http://wap.yfazqb.com/Article/details/gjxpclwhz.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.vehdjk.com/Article/details/gjpvfqlud.sHtML

[U65] PHP：会话
来源：http://www.blog.fktsv.cn/Article/details/glrsdbiir.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.vehdjk.com/Article/details/gmyitbszw.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.yfazqb.com/Article/details/gelcpxvsu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.sjlbkw.cn/Article/details/gzexsyyad.sHtML

[U67] PHP：处理文件上传
来源：http://wap.yfazqb.com/Article/details/gurowgqvx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.yfazqb.com/Article/details/gxwixqtxh.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fktsv.cn/Article/details/grzwhnped.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.sjlbkw.cn/Article/details/gbcptyiay.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.epnwcf.com/Article/details/gyctiernb.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.vehdjk.com/Article/details/gxxktxijx.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.fktsv.cn/Article/details/gzcelgsgn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fktsv.cn/Article/details/gbqilitsx.sHtML

[U71] PHP：抛出异常
来源：http://blog.bbcook.cn/Article/details/gagsqxdhs.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.tarul.cn/Article/details/gycuulgse.sHtML

[U72] PHP：写错误日志
来源：http://www.share.tarul.cn/Article/details/grrbyigqt.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.tarul.cn/Article/details/guhlnmana.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.tarul.cn/Article/details/gjkmjwzgw.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.tarul.cn/Article/details/gyabwfdhk.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.vehdjk.com/Article/details/gtmuhnltf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.sjlbkw.cn/Article/details/gxaqjubkw.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.yfazqb.com/Article/details/gzwirfdfb.sHtML

composer require psr/container
来源：http://wap.yfazqb.com/Article/details/gdvvnuita.sHtML

[U76] PHP：简单路由
来源：http://www.share.tarul.cn/Article/details/gsszpsmkr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.yfazqb.com/Article/details/gbdytklto.sHtML

[U77] PHP：模板渲染
来源：http://www.share.vehdjk.com/Article/details/gmhtabwti.sHtML

composer require twig/twig
来源：http://wap.tarul.cn/Article/details/gurriugra.sHtML

[U78] PHP：单元测试
来源：http://mobile.epnwcf.com/Article/details/gkufpgcvl.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.epnwcf.com/Article/details/glqeiwxjs.sHtML

[U79] PHP：静态分析
来源：http://mobile.yfazqb.com/Article/details/gkxfgwqys.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.bbcook.cn/Article/details/gmntjqusu.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.tarul.cn/Article/details/gsmwkjwul.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.sjlbkw.cn/Article/details/gvrndrrtf.sHtML

[U81] JS：初始化项目
来源：http://read.share.fktsv.cn/Article/details/gbvxwhlxj.sHtML

npm init -y;  npm i express
来源：http://m.share.fktsv.cn/Article/details/gomlylzie.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.epnwcf.com/Article/details/gfdikbugq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.epnwcf.com/Article/details/gkuvlnmmt.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.tarul.cn/Article/details/gzzhdrywh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fktsv.cn/Article/details/ggzhsfhym.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.vehdjk.com/Article/details/giffspscd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.epnwcf.com/Article/details/gnczbbkta.sHtML

[U85] JS：可选链
来源：http://3g.sjlbkw.cn/Article/details/gnhywntbh.sHtML

a?.b?.c
来源：http://m.share.bbcook.cn/Article/details/gujobwqrm.sHtML

[U86] JS：空值合并
来源：http://3g.tarul.cn/Article/details/gksdteamr.sHtML

a ?? b
来源：http://blog.vehdjk.com/Article/details/gykdztwax.sHtML

[U87] JS：解构默认值
来源：http://read.share.sjlbkw.cn/Article/details/gehtdhysd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.epnwcf.com/Article/details/ggamnbaxm.sHtML

[U88] JS：对象展开合并
来源：http://m.share.vehdjk.com/Article/details/gmttaejgy.sHtML

{ ...a, ...b }
来源：http://3g.vehdjk.com/Article/details/ghpnegjas.sHtML

[U89] JS：数组去重
来源：http://3g.fktsv.cn/Article/details/gcdmkkyla.sHtML

[...new Set(arr)]
来源：http://wap.yfazqb.com/Article/details/ggamnnttt.sHtML

[U90] JS：数字数组排序
来源：http://baike.sjlbkw.cn/Article/details/grzkjwlql.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/gmzeaexpr.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fktsv.cn/Article/details/gwbhklpae.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.tarul.cn/Article/details/gkgfpxmqq.sHtML

[U92] JS：深拷贝
来源：http://m.share.vehdjk.com/Article/details/gzcsvzcne.sHtML

structuredClone(obj)
来源：http://m.share.vehdjk.com/Article/details/gveuffgrr.sHtML

[U93] JS：模板字符串
来源：http://www.share.sjlbkw.cn/Article/details/gkmiexjyw.sHtML

`共 ${n} 条`
来源：http://www.share.fktsv.cn/Article/details/gwaabybrr.sHtML

[U94] JS：箭头函数
来源：http://blog.bbcook.cn/Article/details/gsisxfmja.sHtML

const double = x => x * 2;
来源：http://read.share.epnwcf.com/Article/details/grlctlkhz.sHtML

[U95] JS：Promise 包装
来源：http://3g.tarul.cn/Article/details/ghtzmcrif.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.bbcook.cn/Article/details/giyjgrwfg.sHtML

[U96] JS：async/await 与异常
来源：http://wap.tarul.cn/Article/details/gqggdkqio.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gflhrmjja.sHtML

[U97] JS：并发请求
来源：http://read.share.bbcook.cn/Article/details/grskzkawe.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.epnwcf.com/Article/details/getimbzae.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.yfazqb.com/Article/details/gcemzqluf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.sjlbkw.cn/Article/details/gfwfxibwp.sHtML

[U99] JS：事件监听
来源：http://baike.tarul.cn/Article/details/gslhwrzrb.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.epnwcf.com/Article/details/gythvjyih.sHtML

[U100] JS：DOM 查询
来源：http://www.share.vehdjk.com/Article/details/gmnagrdws.sHtML

document.querySelector(".item")
来源：http://www.m.share.vehdjk.com/Article/details/gfpnngnnj.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fktsv.cn/Article/details/gwwjrvdpo.sHtML

el.classList.toggle("active")
来源：http://3g.bbcook.cn/Article/details/glzzearca.sHtML

[U102] JS：本地存储
来源：http://wap.vehdjk.com/Article/details/gnyytvqot.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fktsv.cn/Article/details/gjmntscaw.sHtML

[U103] JS：定时器
来源：http://wap.bbcook.cn/Article/details/gdwrouqvl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.tarul.cn/Article/details/goixitvod.sHtML

[U104] JS：防抖
来源：http://www.m.share.fktsv.cn/Article/details/gitfauqkn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.vehdjk.com/Article/details/gwutcmuin.sHtML

[U105] JS：节流
来源：http://read.share.epnwcf.com/Article/details/gfjleimtw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.bbcook.cn/Article/details/gbmhsokqo.sHtML

[U106] JS：日期格式化
来源：http://mobile.sjlbkw.cn/Article/details/gmhjmynog.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.bbcook.cn/Article/details/ghvfohqum.sHtML

[U107] JS：数字千分位
来源：http://3g.fktsv.cn/Article/details/goqckztfw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.bbcook.cn/Article/details/gdtdzehvc.sHtML

[U108] JS：随机整数
来源：http://mobile.epnwcf.com/Article/details/glokoizlz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.bbcook.cn/Article/details/godhfsvlv.sHtML

[U109] JS：数组分组
来源：http://www.blog.vehdjk.com/Article/details/ghyircodx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.epnwcf.com/Article/details/gbninrzjd.sHtML

[U110] JS：数组分块
来源：http://mobile.sjlbkw.cn/Article/details/gkymfhroc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fktsv.cn/Article/details/gucthgvka.sHtML

[U111] JS：对象转 Map
来源：http://baike.tarul.cn/Article/details/ggjmxmxud.sHtML

new Map(Object.entries(obj))
来源：http://wap.bbcook.cn/Article/details/gdarfskwj.sHtML

[U112] JS：字符串补位
来源：http://mobile.vehdjk.com/Article/details/gjrqsqvde.sHtML

"7".padStart(3, "0")
来源：http://www.share.epnwcf.com/Article/details/gqmujbtaw.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fktsv.cn/Article/details/gjppmsdfp.sHtML

s.replaceAll("a", "b")
来源：http://wap.fktsv.cn/Article/details/gfrfkthem.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.tarul.cn/Article/details/ggymnlucc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.tarul.cn/Article/details/gakrhxkrh.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.sjlbkw.cn/Article/details/guwgfakjy.sHtML

crypto.randomUUID()
来源：http://read.share.vehdjk.com/Article/details/gstushpbd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.tarul.cn/Article/details/gitpouxwe.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.epnwcf.com/Article/details/gxonoefpq.sHtML

[U117] JS：单元测试
来源：http://3g.bbcook.cn/Article/details/gvjtjsptk.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.vehdjk.com/Article/details/gskxqayra.sHtML

[U118] JS：开发服务器
来源：http://m.share.fktsv.cn/Article/details/gxneodufs.sHtML

npm i -D vite;  npx vite
来源：http://3g.yfazqb.com/Article/details/gzcsxxqji.sHtML

[U119] JS：生产构建
来源：http://www.blog.epnwcf.com/Article/details/gwhkslnfp.sHtML

npx vite build
来源：http://blog.fktsv.cn/Article/details/gftrqdcxf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.tarul.cn/Article/details/gugqaldfp.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.sjlbkw.cn/Article/details/gwpddoebj.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gdlqzcuhx.sHtML

统计汇总
来源：http://www.blog.epnwcf.com/Article/details/grslwlsek.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ggpclmhwo.sHtML

按语言统计（条）：
来源：http://www.share.epnwcf.com/Article/details/gfwhehqhj.sHtML

Python ......... 252
来源：http://mobile.epnwcf.com/Article/details/gaikmixls.sHtML

PHP ............ 252
来源：http://mobile.tarul.cn/Article/details/gwtgvsiez.sHtML

JavaScript ..... 252
来源：http://m.share.tarul.cn/Article/details/gtvokruae.sHtML

TypeScript ..... 212
来源：http://www.m.share.bbcook.cn/Article/details/gnyqksjhz.sHtML

Java ........... 212
来源：http://m.share.epnwcf.com/Article/details/gzderabpy.sHtML

Go ............. 212
来源：http://wap.yfazqb.com/Article/details/gqwityten.sHtML

Ruby ........... 212
来源：http://read.share.yfazqb.com/Article/details/gpczwrssg.sHtML

C# ............. 212
来源：http://m.share.bbcook.cn/Article/details/gktjvsnvf.sHtML

C .............. 30
来源：http://blog.vehdjk.com/Article/details/gnqjpntlj.sHtML

C++ ............ 30
来源：http://3g.epnwcf.com/Article/details/gyuthhtna.sHtML

SQL ............ 90
来源：http://blog.epnwcf.com/Article/details/gcmjgyyai.sHtML

Bash ........... 80
来源：http://mobile.tarul.cn/Article/details/gwxtjgaeg.sHtML

Kotlin ......... 15
来源：http://read.share.vehdjk.com/Article/details/guhfysrmc.sHtML

Swift .......... 15
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkuacexr.sHtML

Lua ............ 10
来源：http://mobile.vehdjk.com/Article/details/gqmpgwqqk.sHtML

Perl ........... 10
来源：http://baike.bbcook.cn/Article/details/gfnfbvius.sHtML

Scala .......... 10
来源：http://read.share.fktsv.cn/Article/details/gkmjogcnz.sHtML

------------------------------------
来源：http://3g.vehdjk.com/Article/details/gvaifaoas.sHtML

合计 ........... 2106 条
来源：http://wap.bbcook.cn/Article/details/gvaxzckii.sHtML

按章节统计：
来源：http://3g.sjlbkw.cn/Article/details/gkehxiyfw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.yfazqb.com/Article/details/gomafnqtk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.vehdjk.com/Article/details/gzlxvrasu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.epnwcf.com/Article/details/gysggdhuy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.tarul.cn/Article/details/glsnqovgs.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.vehdjk.com/Article/details/gmakdrmgt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.bbcook.cn/Article/details/giqpxoymz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.yfazqb.com/Article/details/gmisfuxgs.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.tarul.cn/Article/details/gvxixgvck.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fktsv.cn/Article/details/grtzsnvoc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.sjlbkw.cn/Article/details/gmakuehhm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gltvkmdid.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.epnwcf.com/Article/details/gvpdmiyab.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.tarul.cn/Article/details/gzlyvcoeo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.sjlbkw.cn/Article/details/gytiapdtx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fktsv.cn/Article/details/ggnboakfz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.epnwcf.com/Article/details/gmctubuhx.sHtML

Q SQL 专题                              90
来源：http://mobile.epnwcf.com/Article/details/goxtzqndq.sHtML

R Bash 专题                             80
来源：http://m.share.sjlbkw.cn/Article/details/giaefzpqw.sHtML

S C / C++ 专题                          60
来源：http://m.share.yfazqb.com/Article/details/gyuejwkrt.sHtML

T 其他语言补充                          60
来源：http://www.share.bbcook.cn/Article/details/gwjycklcw.sHtML

U 高频实用片段                         120
来源：http://3g.fktsv.cn/Article/details/gshqvobuy.sHtML

------------------------------------
来源：http://mobile.yfazqb.com/Article/details/gymgvbkqi.sHtML

合计                                  2106 条
来源：http://read.share.yfazqb.com/Article/details/gbjowbdso.sHtML

--------------------------------------------------------------------------------
来源：http://blog.tarul.cn/Article/details/genwldawe.sHtML

使用提醒
来源：http://www.share.tarul.cn/Article/details/ghsstkopg.sHtML

--------------------------------------------------------------------------------
来源：http://3g.bbcook.cn/Article/details/gnosjzjss.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fktsv.cn/Article/details/guapzfhgh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fktsv.cn/Article/details/gsjphxwzx.sHtML


<!-- 参考信息 -->