代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://baike.yfazqb.com/Article/details/geirbwwsh.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fktsv.cn/Article/details/gnrwefkve.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.share.yfazqb.com/Article/details/gnltowzlr.sHtML

[T56] Scala：样例类
来源：http://3g.yfazqb.com/Article/details/gzbnhdgrv.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhcizysf.sHtML

[T57] Scala：模式匹配
来源：http://3g.sjlbkw.cn/Article/details/gjyfvmznj.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.tarul.cn/Article/details/gyrnnshgx.sHtML

[T58] Scala：函数定义
来源：http://www.blog.epnwcf.com/Article/details/gzizqwdpt.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.vehdjk.com/Article/details/gnfihhhbr.sHtML

[T59] Scala：循环
来源：http://3g.vehdjk.com/Article/details/gpvuxaqvh.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.sjlbkw.cn/Article/details/gnxhkhmbq.sHtML

[T60] Scala：折叠
来源：http://3g.tarul.cn/Article/details/gczldlbdg.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.yfazqb.com/Article/details/gtfxhlggu.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gnacfktna.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://baike.fktsv.cn/Article/details/guhdjsxyx.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gdgmugaux.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.vehdjk.com/Article/details/gjcncfpij.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://www.m.share.vehdjk.com/Article/details/gtlzhppar.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.vehdjk.com/Article/details/gzcdmsbms.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://blog.fktsv.cn/Article/details/gwzgxzcak.sHtML

[U03] Py：加载 .env 配置
来源：http://mobile.vehdjk.com/Article/details/gsdftzbyf.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.sjlbkw.cn/Article/details/gphfsxepr.sHtML

[U04] Py：变量调试打印
来源：http://www.blog.bbcook.cn/Article/details/gbvqygxfm.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.epnwcf.com/Article/details/gixkiohgs.sHtML

[U05] Py：列表去重且保序
来源：http://mobile.bbcook.cn/Article/details/gdtsbnigl.sHtML

list(dict.fromkeys(arr))
来源：http://baike.sjlbkw.cn/Article/details/gwqctfmly.sHtML

[U06] Py：合并两个字典
来源：http://www.m.share.epnwcf.com/Article/details/gvrdpjleb.sHtML

{**a, **b}
来源：http://m.share.vehdjk.com/Article/details/grsuwmgxe.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.epnwcf.com/Article/details/gwgxefltn.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.fktsv.cn/Article/details/gfvxpwdgd.sHtML

[U08] Py：展平二维列表
来源：http://m.share.tarul.cn/Article/details/grqdtkbbw.sHtML

[y for x in nested for y in x]
来源：http://baike.fktsv.cn/Article/details/gabdeorqk.sHtML

[U09] Py：字典取最大值的键
来源：http://mobile.fktsv.cn/Article/details/ghenrqmuu.sHtML

max(d, key=d.get)
来源：http://www.share.yfazqb.com/Article/details/gxtopvjhh.sHtML

[U10] Py：按值排序字典
来源：http://blog.vehdjk.com/Article/details/gbbgoymmp.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.m.share.yfazqb.com/Article/details/gxmlokixk.sHtML

[U11] Py：生成器表达式
来源：http://3g.bbcook.cn/Article/details/gceawjdli.sHtML

(x * 2 for x in arr)
来源：http://baike.tarul.cn/Article/details/gvuwavmhx.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://baike.bbcook.cn/Article/details/gzcbnyboj.sHtML

Counter(arr).most_common(3)
来源：http://read.share.tarul.cn/Article/details/gyizeetwh.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fktsv.cn/Article/details/gyqipmnxn.sHtML

deque(maxlen=10)
来源：http://wap.vehdjk.com/Article/details/gzfaqyptw.sHtML

[U14] Py：分组收集到列表
来源：http://www.share.bbcook.cn/Article/details/ghstbfdoy.sHtML

defaultdict(list)
来源：http://mobile.fktsv.cn/Article/details/gjkmkzrwe.sHtML

[U15] Py：高精度计时
来源：http://www.share.tarul.cn/Article/details/gcaalkcnb.sHtML

t = time.perf_counter()
来源：http://www.blog.bbcook.cn/Article/details/glgcmtyhp.sHtML

[U16] Py：命令行参数解析
来源：http://www.m.share.tarul.cn/Article/details/gifupawuw.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.share.bbcook.cn/Article/details/gfevuzmen.sHtML

[U17] Py：初始化日志
来源：http://baike.tarul.cn/Article/details/grimzqbur.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.vehdjk.com/Article/details/ghqonrdrh.sHtML

[U18] Py：预编译正则
来源：http://www.blog.fktsv.cn/Article/details/gpbxiablo.sHtML

pat = re.compile(r"\d+")
来源：http://www.blog.sjlbkw.cn/Article/details/gmtbeqfus.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.tarul.cn/Article/details/gwjdamqig.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.tarul.cn/Article/details/gizmifqrr.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.epnwcf.com/Article/details/gbyqoxsdy.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.epnwcf.com/Article/details/ggrngxsab.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.yfazqb.com/Article/details/gjeegvisd.sHtML

@contextlib.contextmanager
来源：http://www.m.share.tarul.cn/Article/details/gobnolbeq.sHtML

[U22] Py：矩阵转置
来源：http://www.share.tarul.cn/Article/details/ghvxgwufl.sHtML

list(zip(*m))
来源：http://3g.bbcook.cn/Article/details/gnyjvuyst.sHtML

[U23] Py：分块读取大文件
来源：http://mobile.epnwcf.com/Article/details/gpwulfsmt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.fktsv.cn/Article/details/gtcvwytmf.sHtML

[U24] Py：路径操作
来源：http://wap.tarul.cn/Article/details/gujjsskff.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wap.yfazqb.com/Article/details/gvaunrozl.sHtML

[U25] Py：CSV 按字典读
来源：http://wap.fktsv.cn/Article/details/gzlwityfl.sHtML

csv.DictReader(f)
来源：http://blog.tarul.cn/Article/details/gmsvmgfel.sHtML

[U26] Py：并发下载
来源：http://baike.bbcook.cn/Article/details/grlrrghte.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.sjlbkw.cn/Article/details/ghauznuym.sHtML

[U27] Py：异步 HTTP
来源：http://www.blog.bbcook.cn/Article/details/gyxjtjksd.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.epnwcf.com/Article/details/gccpnfyrw.sHtML

[U28] Py：类型别名
来源：http://mobile.fktsv.cn/Article/details/gevghnlps.sHtML

UserId = int
来源：http://wap.tarul.cn/Article/details/gnvevzfkg.sHtML

[U29] Py：属性校验
来源：http://3g.bbcook.cn/Article/details/grfqzztgk.sHtML

@property 与 @x.setter 配合
来源：http://www.share.epnwcf.com/Article/details/gjmljhlin.sHtML

[U30] Py：数据类
来源：http://wap.sjlbkw.cn/Article/details/gueljkyzn.sHtML

@dataclass(slots=True)
来源：http://www.share.sjlbkw.cn/Article/details/ghtzysxsu.sHtML

[U31] Py：单测
来源：http://3g.epnwcf.com/Article/details/gyheybabd.sHtML

python -m pytest -q
来源：http://3g.bbcook.cn/Article/details/gyaqrodbo.sHtML

[U32] Py：代码格式化
来源：http://blog.sjlbkw.cn/Article/details/gxlbomzbd.sHtML

ruff format . && ruff check --fix .
来源：http://m.share.bbcook.cn/Article/details/gscyqgqjm.sHtML

[U33] Py：打包发布
来源：http://m.share.fktsv.cn/Article/details/gunmydufb.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.bbcook.cn/Article/details/gfkztddac.sHtML

[U34] Py：判断编码
来源：http://wap.tarul.cn/Article/details/gxwdapnso.sHtML

chardet.detect(raw)
来源：http://mobile.tarul.cn/Article/details/gbszjvvti.sHtML

[U35] Py：发送邮件
来源：http://www.share.fktsv.cn/Article/details/gfpuoffiz.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.share.yfazqb.com/Article/details/gskugbvpb.sHtML

[U36] Py：定时任务
来源：http://www.m.share.yfazqb.com/Article/details/glthrzfeu.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.yfazqb.com/Article/details/geheicngm.sHtML

[U37] Py：读写 Excel
来源：http://read.share.fktsv.cn/Article/details/gqirjugef.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://blog.yfazqb.com/Article/details/gernyadqm.sHtML

[U38] Py：获取脚本所在目录
来源：http://mobile.fktsv.cn/Article/details/goafgdexr.sHtML

Path(__file__).resolve().parent
来源：http://blog.fktsv.cn/Article/details/gklejbwxw.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.epnwcf.com/Article/details/geqpdoshc.sHtML

sys.stdout.isatty()
来源：http://baike.bbcook.cn/Article/details/glnjiizje.sHtML

[U40] Py：打印到标准错误
来源：http://m.share.bbcook.cn/Article/details/ggflgbydu.sHtML

print("err", file=sys.stderr)
来源：http://www.m.share.tarul.cn/Article/details/glwddsfgo.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.epnwcf.com/Article/details/gkwhoqxyq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.yfazqb.com/Article/details/gsgolmlna.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.fktsv.cn/Article/details/gbgcxeqos.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.tarul.cn/Article/details/gxxzrwtxz.sHtML

[U43] PHP：声明命名空间
来源：http://wap.bbcook.cn/Article/details/gucwqjkat.sHtML

namespace App\Http;
来源：http://wap.tarul.cn/Article/details/gfcihwfjy.sHtML

[U44] PHP：开启严格类型
来源：http://wap.sjlbkw.cn/Article/details/glykcxqsf.sHtML

declare(strict_types=1);
来源：http://www.blog.epnwcf.com/Article/details/gduutnsll.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.fktsv.cn/Article/details/gpetjirti.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.epnwcf.com/Article/details/gamidbrtv.sHtML

[U46] PHP：可空类型
来源：http://www.blog.tarul.cn/Article/details/geufeddpc.sHtML

?string $name = null
来源：http://www.blog.fktsv.cn/Article/details/gdvgqessd.sHtML

[U47] PHP：联合类型
来源：http://m.share.vehdjk.com/Article/details/glrketink.sHtML

int|string $id
来源：http://blog.sjlbkw.cn/Article/details/grbeolnpg.sHtML

[U48] PHP：纯枚举
来源：http://m.share.tarul.cn/Article/details/gjmtzqexr.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.sjlbkw.cn/Article/details/gmwgfeqci.sHtML

[U49] PHP：只读属性
来源：http://mobile.tarul.cn/Article/details/gwhvndngh.sHtML

public readonly string $name
来源：http://3g.vehdjk.com/Article/details/gskjzeznt.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.tarul.cn/Article/details/gymtzqcwx.sHtML

public function __construct(private int $id) {}
来源：http://wap.tarul.cn/Article/details/gxmdhbswr.sHtML

[U51] PHP：数组解构
来源：http://www.blog.yfazqb.com/Article/details/gpbnhlsgl.sHtML

[$a, $b] = $arr;
来源：http://baike.sjlbkw.cn/Article/details/gqijawzre.sHtML

[U52] PHP：箭头函数
来源：http://read.share.bbcook.cn/Article/details/gplguwphj.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fktsv.cn/Article/details/grmjwgume.sHtML

[U53] PHP：空合并运算符
来源：http://blog.yfazqb.com/Article/details/gstjkhtty.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.sjlbkw.cn/Article/details/gfzhcubtl.sHtML

[U54] PHP：空安全调用
来源：http://wap.fktsv.cn/Article/details/gzywsyhtz.sHtML

$obj?->method()
来源：http://blog.tarul.cn/Article/details/gijhimccl.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gciawjcnz.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.bbcook.cn/Article/details/gdkntnfik.sHtML

[U56] PHP：命名参数
来源：http://blog.fktsv.cn/Article/details/gtbtnkatw.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.yfazqb.com/Article/details/ganikncpv.sHtML

[U57] PHP：字符串插值
来源：http://wap.bbcook.cn/Article/details/gzfrfncmv.sHtML

"值: {$a}"
来源：http://mobile.fktsv.cn/Article/details/godyzpnjr.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.vehdjk.com/Article/details/gxvdkxcqv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.vehdjk.com/Article/details/grnibakdz.sHtML

[U59] PHP：自定义排序
来源：http://mobile.fktsv.cn/Article/details/gnlgvaodu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.tarul.cn/Article/details/gcgithvtd.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.sjlbkw.cn/Article/details/gewnmtqsm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.blog.sjlbkw.cn/Article/details/gbdbtecbl.sHtML

[U61] PHP：正则
来源：http://wap.tarul.cn/Article/details/gnfqddlrp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.epnwcf.com/Article/details/ggibajadi.sHtML

[U62] PHP：日期对象
来源：http://3g.bbcook.cn/Article/details/gesvqinjw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.sjlbkw.cn/Article/details/glwecxsge.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.tarul.cn/Article/details/ghygdyzhr.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.epnwcf.com/Article/details/gwpfxqkqm.sHtML

[U64] PHP：目录遍历
来源：http://m.share.epnwcf.com/Article/details/gpfmyqvgg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fktsv.cn/Article/details/gmelxrbqy.sHtML

[U65] PHP：会话
来源：http://read.share.yfazqb.com/Article/details/gkgnjnnou.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.bbcook.cn/Article/details/gkzapuehj.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.bbcook.cn/Article/details/gxhdwejfc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.tarul.cn/Article/details/gyyskbaiy.sHtML

[U67] PHP：处理文件上传
来源：http://3g.tarul.cn/Article/details/gfysrbbcl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.vehdjk.com/Article/details/gndpqudsp.sHtML

[U68] PHP：PDO 连接
来源：http://3g.yfazqb.com/Article/details/gwolvcufs.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.tarul.cn/Article/details/gkcuvnjbt.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.sjlbkw.cn/Article/details/gngvyhahr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.yfazqb.com/Article/details/gehcpgdbn.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.bbcook.cn/Article/details/gsczaaksz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.yfazqb.com/Article/details/gdibdmuqg.sHtML

[U71] PHP：抛出异常
来源：http://m.share.vehdjk.com/Article/details/gngzcjbbg.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.epnwcf.com/Article/details/gvqirdthn.sHtML

[U72] PHP：写错误日志
来源：http://wap.fktsv.cn/Article/details/gnbmbtwfi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.vehdjk.com/Article/details/girjmcnia.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.sjlbkw.cn/Article/details/gbttuyqmm.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.epnwcf.com/Article/details/gmzimqfii.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.yfazqb.com/Article/details/ggwctajdr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.bbcook.cn/Article/details/gjkijifza.sHtML

[U75] PHP：依赖注入
来源：http://baike.sjlbkw.cn/Article/details/ghdgvrcfy.sHtML

composer require psr/container
来源：http://www.blog.yfazqb.com/Article/details/gfuylgyik.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.sjlbkw.cn/Article/details/giydezikb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.yfazqb.com/Article/details/gyvpudsaz.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fktsv.cn/Article/details/grmbbniou.sHtML

composer require twig/twig
来源：http://blog.bbcook.cn/Article/details/gmyioxllv.sHtML

[U78] PHP：单元测试
来源：http://blog.bbcook.cn/Article/details/gufzqugpu.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fktsv.cn/Article/details/grbkzfqyb.sHtML

[U79] PHP：静态分析
来源：http://read.share.sjlbkw.cn/Article/details/gheoililx.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.epnwcf.com/Article/details/gttegzlfw.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.tarul.cn/Article/details/gmzsygrgd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.bbcook.cn/Article/details/gwkhpmwqz.sHtML

[U81] JS：初始化项目
来源：http://wap.tarul.cn/Article/details/gqwighaod.sHtML

npm init -y;  npm i express
来源：http://baike.fktsv.cn/Article/details/grzjpxmbf.sHtML

[U82] JS：package.json 脚本
来源：http://3g.yfazqb.com/Article/details/ghrixabwi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.vehdjk.com/Article/details/gzlgdncgi.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.vehdjk.com/Article/details/gxezznjdk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.bbcook.cn/Article/details/gvrbxenhn.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.vehdjk.com/Article/details/gchtdpxsw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.bbcook.cn/Article/details/gegfbjeeo.sHtML

[U85] JS：可选链
来源：http://www.blog.tarul.cn/Article/details/gisbsradm.sHtML

a?.b?.c
来源：http://3g.vehdjk.com/Article/details/gzlntzsrf.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fktsv.cn/Article/details/gcwbbvhap.sHtML

a ?? b
来源：http://wap.sjlbkw.cn/Article/details/gsmgrrnwh.sHtML

[U87] JS：解构默认值
来源：http://www.share.sjlbkw.cn/Article/details/gjcqfgigd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.sjlbkw.cn/Article/details/gbhjybjxa.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.epnwcf.com/Article/details/gzcbhtwjc.sHtML

{ ...a, ...b }
来源：http://mobile.yfazqb.com/Article/details/gmstsoqiy.sHtML

[U89] JS：数组去重
来源：http://wap.epnwcf.com/Article/details/gaobatdkf.sHtML

[...new Set(arr)]
来源：http://www.blog.vehdjk.com/Article/details/gilkfsydw.sHtML

[U90] JS：数字数组排序
来源：http://www.share.sjlbkw.cn/Article/details/gygiouzsq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/gcnqtbczs.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.vehdjk.com/Article/details/gnwgombnh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.tarul.cn/Article/details/gijxocspv.sHtML

[U92] JS：深拷贝
来源：http://www.blog.tarul.cn/Article/details/gsxanerfw.sHtML

structuredClone(obj)
来源：http://www.m.share.tarul.cn/Article/details/gsugmgobn.sHtML

[U93] JS：模板字符串
来源：http://read.share.bbcook.cn/Article/details/gusyisvdq.sHtML

`共 ${n} 条`
来源：http://read.share.vehdjk.com/Article/details/guelrvdid.sHtML

[U94] JS：箭头函数
来源：http://www.blog.yfazqb.com/Article/details/gfaremlyr.sHtML

const double = x => x * 2;
来源：http://m.share.fktsv.cn/Article/details/gktxwsqxz.sHtML

[U95] JS：Promise 包装
来源：http://mobile.bbcook.cn/Article/details/gnadkjcgj.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.yfazqb.com/Article/details/gvnaqnhxw.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.yfazqb.com/Article/details/gizbzzsda.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.yfazqb.com/Article/details/gqdwkimvz.sHtML

[U97] JS：并发请求
来源：http://www.share.bbcook.cn/Article/details/gzoezybgm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/gwwwzpowi.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fktsv.cn/Article/details/gydveqiml.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.yfazqb.com/Article/details/gxngsnylo.sHtML

[U99] JS：事件监听
来源：http://read.share.vehdjk.com/Article/details/gbqibtrmq.sHtML

el.addEventListener("click", e => {})
来源：http://baike.tarul.cn/Article/details/gqvcoteme.sHtML

[U100] JS：DOM 查询
来源：http://3g.bbcook.cn/Article/details/gyayknoic.sHtML

document.querySelector(".item")
来源：http://mobile.sjlbkw.cn/Article/details/gxmlzpewh.sHtML

[U101] JS：classList 操作
来源：http://www.blog.tarul.cn/Article/details/guniqmudf.sHtML

el.classList.toggle("active")
来源：http://www.blog.tarul.cn/Article/details/gbjaqxisp.sHtML

[U102] JS：本地存储
来源：http://baike.sjlbkw.cn/Article/details/gghingkvd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fktsv.cn/Article/details/gfpssxxzx.sHtML

[U103] JS：定时器
来源：http://read.share.vehdjk.com/Article/details/gxpcuzkys.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.tarul.cn/Article/details/gwajogoge.sHtML

[U104] JS：防抖
来源：http://www.blog.fktsv.cn/Article/details/gdqotqaaj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.epnwcf.com/Article/details/gaixgqgsh.sHtML

[U105] JS：节流
来源：http://blog.bbcook.cn/Article/details/gzlwzmavv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.tarul.cn/Article/details/gjnmfovnf.sHtML

[U106] JS：日期格式化
来源：http://3g.tarul.cn/Article/details/gyjbcpllk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.sjlbkw.cn/Article/details/gxldrgtlg.sHtML

[U107] JS：数字千分位
来源：http://www.share.sjlbkw.cn/Article/details/ghrnjfifu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.vehdjk.com/Article/details/gtrocbxbw.sHtML

[U108] JS：随机整数
来源：http://read.share.bbcook.cn/Article/details/geupkceca.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.yfazqb.com/Article/details/gpouyimuu.sHtML

[U109] JS：数组分组
来源：http://www.share.tarul.cn/Article/details/gguoeayqz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.bbcook.cn/Article/details/gfenpicmf.sHtML

[U110] JS：数组分块
来源：http://read.share.sjlbkw.cn/Article/details/glspnvcga.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.yfazqb.com/Article/details/gycrjzffh.sHtML

[U111] JS：对象转 Map
来源：http://www.share.yfazqb.com/Article/details/gcintnskc.sHtML

new Map(Object.entries(obj))
来源：http://wap.bbcook.cn/Article/details/grjnhvkwd.sHtML

[U112] JS：字符串补位
来源：http://read.share.bbcook.cn/Article/details/gdcvdfxne.sHtML

"7".padStart(3, "0")
来源：http://mobile.fktsv.cn/Article/details/guyioinix.sHtML

[U113] JS：正则替换全部
来源：http://wap.fktsv.cn/Article/details/gtuqkpxsk.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.bbcook.cn/Article/details/gfmqbhgzn.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.vehdjk.com/Article/details/gqlqhejpa.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.bbcook.cn/Article/details/gkwbjsdkl.sHtML

[U115] JS：生成 UUID
来源：http://read.share.tarul.cn/Article/details/gorbdyhfx.sHtML

crypto.randomUUID()
来源：http://3g.sjlbkw.cn/Article/details/gjxpgycnd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.yfazqb.com/Article/details/gacokmjal.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.bbcook.cn/Article/details/gfaimovol.sHtML

[U117] JS：单元测试
来源：http://baike.epnwcf.com/Article/details/gpxjznrhq.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.sjlbkw.cn/Article/details/gekkukqpk.sHtML

[U118] JS：开发服务器
来源：http://baike.tarul.cn/Article/details/gqicujexh.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.yfazqb.com/Article/details/gfvgvolbx.sHtML

[U119] JS：生产构建
来源：http://mobile.bbcook.cn/Article/details/gucejench.sHtML

npx vite build
来源：http://blog.yfazqb.com/Article/details/gwrlewmgy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.sjlbkw.cn/Article/details/gcsiclphq.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.tarul.cn/Article/details/ghskgncfe.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gtpznpfyh.sHtML

统计汇总
来源：http://www.blog.tarul.cn/Article/details/gepnaxvzt.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gleybvnjx.sHtML

按语言统计（条）：
来源：http://wap.vehdjk.com/Article/details/gsfjrikhh.sHtML

Python ......... 252
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzuaeber.sHtML

PHP ............ 252
来源：http://mobile.sjlbkw.cn/Article/details/gsbtdcyrw.sHtML

JavaScript ..... 252
来源：http://www.m.share.yfazqb.com/Article/details/gyflaohth.sHtML

TypeScript ..... 212
来源：http://blog.epnwcf.com/Article/details/gbzjzkyqq.sHtML

Java ........... 212
来源：http://baike.yfazqb.com/Article/details/gpvuvzbfl.sHtML

Go ............. 212
来源：http://read.share.epnwcf.com/Article/details/gzadtokpl.sHtML

Ruby ........... 212
来源：http://wap.vehdjk.com/Article/details/gemxjpgmo.sHtML

C# ............. 212
来源：http://mobile.bbcook.cn/Article/details/gdqybwqsf.sHtML

C .............. 30
来源：http://www.blog.bbcook.cn/Article/details/gsunmfiqa.sHtML

C++ ............ 30
来源：http://www.share.bbcook.cn/Article/details/gdqclvqfp.sHtML

SQL ............ 90
来源：http://www.share.vehdjk.com/Article/details/gqyshmeef.sHtML

Bash ........... 80
来源：http://mobile.tarul.cn/Article/details/gnrprqbbt.sHtML

Kotlin ......... 15
来源：http://www.share.yfazqb.com/Article/details/gdackdkuv.sHtML

Swift .......... 15
来源：http://3g.epnwcf.com/Article/details/gscqqutkr.sHtML

Lua ............ 10
来源：http://m.share.sjlbkw.cn/Article/details/gncskaiqk.sHtML

Perl ........... 10
来源：http://3g.vehdjk.com/Article/details/gkqdxglih.sHtML

Scala .......... 10
来源：http://baike.epnwcf.com/Article/details/gdtzpkwrl.sHtML

------------------------------------
来源：http://wap.epnwcf.com/Article/details/gzqbmdjbu.sHtML

合计 ........... 2106 条
来源：http://blog.epnwcf.com/Article/details/gjyyzcgva.sHtML

按章节统计：
来源：http://baike.bbcook.cn/Article/details/gdgexodqz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.yfazqb.com/Article/details/guctwerow.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.sjlbkw.cn/Article/details/goolgudvu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.sjlbkw.cn/Article/details/gsqakwmkc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fktsv.cn/Article/details/gqaftmyhz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.bbcook.cn/Article/details/gvxjdhewq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.sjlbkw.cn/Article/details/glzgxarqg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.epnwcf.com/Article/details/gyyguyyzu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.tarul.cn/Article/details/gjupeqsws.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.yfazqb.com/Article/details/ggurowelv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.sjlbkw.cn/Article/details/ghualicxr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.tarul.cn/Article/details/gkcnltvoz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.yfazqb.com/Article/details/gfuxamjfy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.yfazqb.com/Article/details/ggxobdzah.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.sjlbkw.cn/Article/details/gviivgtbt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.epnwcf.com/Article/details/gfychoocl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.sjlbkw.cn/Article/details/ghgvgphpy.sHtML

Q SQL 专题                              90
来源：http://www.m.share.epnwcf.com/Article/details/grflgkzoo.sHtML

R Bash 专题                             80
来源：http://baike.tarul.cn/Article/details/ghkmxiobu.sHtML

S C / C++ 专题                          60
来源：http://blog.sjlbkw.cn/Article/details/gyuoftjgo.sHtML

T 其他语言补充                          60
来源：http://read.share.tarul.cn/Article/details/gqbfhzjet.sHtML


<!-- 参考信息 -->