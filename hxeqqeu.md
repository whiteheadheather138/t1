代发 wailian999

List(1, 2, 3).map(_ * 2)
来源：http://wap.sjlbkw.cn/Article/details/gdfusaxoo.sHtML

[T55] Scala：集合过滤
来源：http://baike.bbcook.cn/Article/details/gkjizycsa.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fktsv.cn/Article/details/gpvebuahe.sHtML

[T56] Scala：样例类
来源：http://read.share.yfazqb.com/Article/details/gtiunumdj.sHtML

case class User(name: String, age: Int)
来源：http://www.share.vehdjk.com/Article/details/gxcchygex.sHtML

[T57] Scala：模式匹配
来源：http://wap.vehdjk.com/Article/details/gnnipymgk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.epnwcf.com/Article/details/gwilkxxxq.sHtML

[T58] Scala：函数定义
来源：http://read.share.bbcook.cn/Article/details/gschwdkrk.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.vehdjk.com/Article/details/gshyynsvb.sHtML

[T59] Scala：循环
来源：http://blog.fktsv.cn/Article/details/gateddlim.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.share.bbcook.cn/Article/details/gvfrboxme.sHtML

[T60] Scala：折叠
来源：http://3g.sjlbkw.cn/Article/details/gxqmvkjxm.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.yfazqb.com/Article/details/gfjtwhklk.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gjhomifpx.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.tarul.cn/Article/details/glpprviyc.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gyvgoglvb.sHtML

[U01] Py：创建虚拟环境
来源：http://read.share.tarul.cn/Article/details/gsqsbzcgd.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://m.share.bbcook.cn/Article/details/ghvurejer.sHtML

[U02] Py：导出 / 安装依赖
来源：http://www.share.vehdjk.com/Article/details/gowdmwgua.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.fktsv.cn/Article/details/gwaazbqml.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fktsv.cn/Article/details/gdterwzru.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.vehdjk.com/Article/details/gqmilqhtq.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.bbcook.cn/Article/details/gwwanftaq.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.tarul.cn/Article/details/gahqowplc.sHtML

[U05] Py：列表去重且保序
来源：http://www.share.vehdjk.com/Article/details/gsoybrqcq.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.bbcook.cn/Article/details/gymjuzmvo.sHtML

[U06] Py：合并两个字典
来源：http://www.share.sjlbkw.cn/Article/details/gpdyrxbvb.sHtML

{**a, **b}
来源：http://blog.epnwcf.com/Article/details/grlulshgo.sHtML

[U07] Py：反转字典键值
来源：http://m.share.bbcook.cn/Article/details/gpihaevjx.sHtML

{v: k for k, v in d.items()}
来源：http://m.share.epnwcf.com/Article/details/gwskkbvhd.sHtML

[U08] Py：展平二维列表
来源：http://www.share.tarul.cn/Article/details/gjvfzqven.sHtML

[y for x in nested for y in x]
来源：http://wap.vehdjk.com/Article/details/gldtattph.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.fktsv.cn/Article/details/gqtmfwsal.sHtML

max(d, key=d.get)
来源：http://mobile.sjlbkw.cn/Article/details/gdhzekcqc.sHtML

[U10] Py：按值排序字典
来源：http://mobile.epnwcf.com/Article/details/gwkwcmxyn.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wap.epnwcf.com/Article/details/gzxdzjqai.sHtML

[U11] Py：生成器表达式
来源：http://baike.tarul.cn/Article/details/gdfcpykxg.sHtML

(x * 2 for x in arr)
来源：http://baike.vehdjk.com/Article/details/gptssdhsa.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.tarul.cn/Article/details/gqwkmkjbm.sHtML

Counter(arr).most_common(3)
来源：http://baike.bbcook.cn/Article/details/gzmotmfxj.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.fktsv.cn/Article/details/gxgbtrmrz.sHtML

deque(maxlen=10)
来源：http://baike.sjlbkw.cn/Article/details/gdyavalxj.sHtML

[U14] Py：分组收集到列表
来源：http://read.share.epnwcf.com/Article/details/guohoalbv.sHtML

defaultdict(list)
来源：http://3g.yfazqb.com/Article/details/gcyuybedn.sHtML

[U15] Py：高精度计时
来源：http://www.m.share.epnwcf.com/Article/details/gcfvxhkas.sHtML

t = time.perf_counter()
来源：http://www.share.yfazqb.com/Article/details/gxugtnumb.sHtML

[U16] Py：命令行参数解析
来源：http://3g.yfazqb.com/Article/details/grjawipmj.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://3g.yfazqb.com/Article/details/giiieodqq.sHtML

[U17] Py：初始化日志
来源：http://3g.tarul.cn/Article/details/gmxddxauo.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://m.share.fktsv.cn/Article/details/gejaqdpho.sHtML

[U18] Py：预编译正则
来源：http://wap.epnwcf.com/Article/details/gmaynlghv.sHtML

pat = re.compile(r"\d+")
来源：http://blog.epnwcf.com/Article/details/gbgcdcevr.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fktsv.cn/Article/details/grxoxzduo.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.blog.fktsv.cn/Article/details/gvqxjczum.sHtML

[U20] Py：缓存函数结果
来源：http://read.share.sjlbkw.cn/Article/details/gvqjewjct.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.fktsv.cn/Article/details/gfcgrzcec.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.m.share.fktsv.cn/Article/details/gqwnhttip.sHtML

@contextlib.contextmanager
来源：http://baike.tarul.cn/Article/details/gtproqmsi.sHtML

[U22] Py：矩阵转置
来源：http://blog.fktsv.cn/Article/details/glhroxxqg.sHtML

list(zip(*m))
来源：http://baike.sjlbkw.cn/Article/details/gukupxkgj.sHtML

[U23] Py：分块读取大文件
来源：http://wap.tarul.cn/Article/details/gastfvysm.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.vehdjk.com/Article/details/gcdxcocap.sHtML

[U24] Py：路径操作
来源：http://read.share.epnwcf.com/Article/details/glgowricr.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.bbcook.cn/Article/details/gwcsmskez.sHtML

[U25] Py：CSV 按字典读
来源：http://mobile.yfazqb.com/Article/details/gkrkdwcjy.sHtML

csv.DictReader(f)
来源：http://wap.epnwcf.com/Article/details/gkuczhkrf.sHtML

[U26] Py：并发下载
来源：http://wap.epnwcf.com/Article/details/grczzepmr.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.sjlbkw.cn/Article/details/grqxrapad.sHtML

[U27] Py：异步 HTTP
来源：http://3g.bbcook.cn/Article/details/gwotvxsvh.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://mobile.yfazqb.com/Article/details/gxinjqtdt.sHtML

[U28] Py：类型别名
来源：http://m.share.sjlbkw.cn/Article/details/gvqhszigg.sHtML

UserId = int
来源：http://blog.epnwcf.com/Article/details/gukezokvs.sHtML

[U29] Py：属性校验
来源：http://wap.vehdjk.com/Article/details/gdsbhtsjm.sHtML

@property 与 @x.setter 配合
来源：http://www.blog.bbcook.cn/Article/details/gjfjpuyac.sHtML

[U30] Py：数据类
来源：http://wap.epnwcf.com/Article/details/gzpzjtrhk.sHtML

@dataclass(slots=True)
来源：http://baike.epnwcf.com/Article/details/gjmgquqoq.sHtML

[U31] Py：单测
来源：http://read.share.yfazqb.com/Article/details/gughdnshn.sHtML

python -m pytest -q
来源：http://wap.tarul.cn/Article/details/gdqujpuzr.sHtML

[U32] Py：代码格式化
来源：http://wap.vehdjk.com/Article/details/geisontly.sHtML

ruff format . && ruff check --fix .
来源：http://wap.epnwcf.com/Article/details/gcizcjhja.sHtML

[U33] Py：打包发布
来源：http://www.share.bbcook.cn/Article/details/gozbmpqnv.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.vehdjk.com/Article/details/gshpbmllw.sHtML

[U34] Py：判断编码
来源：http://www.share.yfazqb.com/Article/details/genadrumj.sHtML

chardet.detect(raw)
来源：http://www.share.yfazqb.com/Article/details/gvnnimhvq.sHtML

[U35] Py：发送邮件
来源：http://baike.epnwcf.com/Article/details/gijsagbcu.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.fktsv.cn/Article/details/ggjjscdbt.sHtML

[U36] Py：定时任务
来源：http://read.share.tarul.cn/Article/details/gvmuoiddf.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.share.bbcook.cn/Article/details/gvsiuwwbb.sHtML

[U37] Py：读写 Excel
来源：http://www.m.share.bbcook.cn/Article/details/gvwqeygcx.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.blog.sjlbkw.cn/Article/details/gxsxtcwzh.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.sjlbkw.cn/Article/details/gipiuppkg.sHtML

Path(__file__).resolve().parent
来源：http://read.share.sjlbkw.cn/Article/details/ghyppjkqz.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.bbcook.cn/Article/details/gzavbculo.sHtML

sys.stdout.isatty()
来源：http://blog.epnwcf.com/Article/details/gjrrzomvp.sHtML

[U40] Py：打印到标准错误
来源：http://baike.bbcook.cn/Article/details/gcqcqhnha.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.yfazqb.com/Article/details/gehzmifjk.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.bbcook.cn/Article/details/gjyxedytg.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.vehdjk.com/Article/details/gcbzvtfsa.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.fktsv.cn/Article/details/gdnexfldi.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://baike.vehdjk.com/Article/details/ggwhotxyk.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.vehdjk.com/Article/details/gcdsqedmt.sHtML

namespace App\Http;
来源：http://wap.fktsv.cn/Article/details/gxnrgjsqg.sHtML

[U44] PHP：开启严格类型
来源：http://blog.yfazqb.com/Article/details/gyqoneheb.sHtML

declare(strict_types=1);
来源：http://wap.tarul.cn/Article/details/gdrxjawuk.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.sjlbkw.cn/Article/details/gicdtkyhq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.sjlbkw.cn/Article/details/gopmhfbmh.sHtML

[U46] PHP：可空类型
来源：http://blog.epnwcf.com/Article/details/glrbvqddg.sHtML

?string $name = null
来源：http://www.m.share.vehdjk.com/Article/details/gshxkbwdu.sHtML

[U47] PHP：联合类型
来源：http://www.blog.bbcook.cn/Article/details/gxhafvode.sHtML

int|string $id
来源：http://3g.bbcook.cn/Article/details/geuwgibgj.sHtML

[U48] PHP：纯枚举
来源：http://www.share.sjlbkw.cn/Article/details/gtezgttim.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.yfazqb.com/Article/details/gpwoabpha.sHtML

[U49] PHP：只读属性
来源：http://blog.epnwcf.com/Article/details/gpaesjzbi.sHtML

public readonly string $name
来源：http://blog.vehdjk.com/Article/details/gczobjbsh.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.yfazqb.com/Article/details/gcespvbhy.sHtML

public function __construct(private int $id) {}
来源：http://wap.epnwcf.com/Article/details/gmhiqosnc.sHtML

[U51] PHP：数组解构
来源：http://www.blog.tarul.cn/Article/details/gflfwxici.sHtML

[$a, $b] = $arr;
来源：http://baike.yfazqb.com/Article/details/gpzijlzej.sHtML

[U52] PHP：箭头函数
来源：http://mobile.epnwcf.com/Article/details/gquzpahhz.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.epnwcf.com/Article/details/gayvvoojj.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.bbcook.cn/Article/details/gbcygjtus.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fktsv.cn/Article/details/gajbkuvnk.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fktsv.cn/Article/details/ghjmanivp.sHtML

$obj?->method()
来源：http://www.blog.vehdjk.com/Article/details/govvjqnjy.sHtML

[U55] PHP：match 表达式
来源：http://wap.sjlbkw.cn/Article/details/gsegqavjq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mobile.yfazqb.com/Article/details/gzrbhpstv.sHtML

[U56] PHP：命名参数
来源：http://3g.tarul.cn/Article/details/gqhchyvew.sHtML

f(a: 1, b: 2)
来源：http://mobile.epnwcf.com/Article/details/gatooduup.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.fktsv.cn/Article/details/gzjlaaetj.sHtML

"值: {$a}"
来源：http://blog.sjlbkw.cn/Article/details/gwurvmrai.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fktsv.cn/Article/details/ghxhwfznb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.yfazqb.com/Article/details/gzpabjuza.sHtML

[U59] PHP：自定义排序
来源：http://blog.vehdjk.com/Article/details/gjkoarjwc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.vehdjk.com/Article/details/gbrqbtwss.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.tarul.cn/Article/details/gtsnorypr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fktsv.cn/Article/details/gswzgalbm.sHtML

[U61] PHP：正则
来源：http://www.blog.yfazqb.com/Article/details/gjhtobgtg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.sjlbkw.cn/Article/details/gcwgmtanc.sHtML

[U62] PHP：日期对象
来源：http://m.share.sjlbkw.cn/Article/details/gacpgdupj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.bbcook.cn/Article/details/gnaboeuxp.sHtML

[U63] PHP：文件读写
来源：http://blog.fktsv.cn/Article/details/gohcaaiyz.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.epnwcf.com/Article/details/gpmjfdqgr.sHtML

[U64] PHP：目录遍历
来源：http://blog.vehdjk.com/Article/details/gfyuwgysf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.bbcook.cn/Article/details/gcswdcwkv.sHtML

[U65] PHP：会话
来源：http://wap.fktsv.cn/Article/details/gjiyfesev.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.yfazqb.com/Article/details/gtqlvbvwc.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.vehdjk.com/Article/details/gpyicbxaq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.yfazqb.com/Article/details/glgkcgaws.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fktsv.cn/Article/details/glgcwmlmh.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.tarul.cn/Article/details/glhlaffmo.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.fktsv.cn/Article/details/gxikizsao.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.sjlbkw.cn/Article/details/gpnurgjoj.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.bbcook.cn/Article/details/gmsnrahsr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.vehdjk.com/Article/details/guinhljus.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.vehdjk.com/Article/details/gqhynxuom.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.epnwcf.com/Article/details/grhcehnst.sHtML

[U71] PHP：抛出异常
来源：http://blog.tarul.cn/Article/details/ghsqofqqa.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.yfazqb.com/Article/details/gldcskwvb.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.yfazqb.com/Article/details/gvukflmxa.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.bbcook.cn/Article/details/gbtolniii.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.epnwcf.com/Article/details/gujahnsaq.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.sjlbkw.cn/Article/details/gnpumbhmf.sHtML

[U74] PHP：读取环境变量
来源：http://3g.yfazqb.com/Article/details/gjvdpzbli.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.vehdjk.com/Article/details/gsfszcjvz.sHtML

[U75] PHP：依赖注入
来源：http://read.share.epnwcf.com/Article/details/gmwrzxfan.sHtML

composer require psr/container
来源：http://www.blog.sjlbkw.cn/Article/details/gkmrojywi.sHtML

[U76] PHP：简单路由
来源：http://m.share.fktsv.cn/Article/details/gmxktkfqh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.sjlbkw.cn/Article/details/gjkvvdjbr.sHtML

[U77] PHP：模板渲染
来源：http://m.share.vehdjk.com/Article/details/gmpoyeuss.sHtML

composer require twig/twig
来源：http://blog.fktsv.cn/Article/details/gkzbwivyy.sHtML

[U78] PHP：单元测试
来源：http://3g.tarul.cn/Article/details/gjbrcwrhc.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.tarul.cn/Article/details/gqqdvycbr.sHtML

[U79] PHP：静态分析
来源：http://wap.sjlbkw.cn/Article/details/gnejyxuio.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fktsv.cn/Article/details/ghkxirejn.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.sjlbkw.cn/Article/details/gggfmkzwo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.bbcook.cn/Article/details/gvgweeqeb.sHtML

[U81] JS：初始化项目
来源：http://3g.vehdjk.com/Article/details/gtfhjfhrg.sHtML

npm init -y;  npm i express
来源：http://www.blog.epnwcf.com/Article/details/gpdbfptsw.sHtML

[U82] JS：package.json 脚本
来源：http://baike.tarul.cn/Article/details/gshswtwua.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.bbcook.cn/Article/details/gurrmmeug.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.bbcook.cn/Article/details/ggithlgur.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.bbcook.cn/Article/details/gqjvhkukc.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.tarul.cn/Article/details/gveltliuw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.sjlbkw.cn/Article/details/goeohmmyr.sHtML

[U85] JS：可选链
来源：http://baike.yfazqb.com/Article/details/gabrlowte.sHtML

a?.b?.c
来源：http://baike.tarul.cn/Article/details/gjfvxqepe.sHtML

[U86] JS：空值合并
来源：http://www.blog.vehdjk.com/Article/details/gplsfdntd.sHtML

a ?? b
来源：http://www.blog.tarul.cn/Article/details/gpqsqewac.sHtML

[U87] JS：解构默认值
来源：http://baike.tarul.cn/Article/details/giaoeuizf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.bbcook.cn/Article/details/gtjjpzznv.sHtML

[U88] JS：对象展开合并
来源：http://mobile.tarul.cn/Article/details/glstvndpo.sHtML

{ ...a, ...b }
来源：http://www.share.bbcook.cn/Article/details/gwhqsugkw.sHtML

[U89] JS：数组去重
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtnmhjqw.sHtML

[...new Set(arr)]
来源：http://mobile.sjlbkw.cn/Article/details/gsbjekrmf.sHtML

[U90] JS：数字数组排序
来源：http://blog.tarul.cn/Article/details/gjwkthrzm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/gsofjmnuh.sHtML

[U91] JS：对象键值遍历
来源：http://baike.epnwcf.com/Article/details/gzfgboggv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.sjlbkw.cn/Article/details/gxvmoihda.sHtML

[U92] JS：深拷贝
来源：http://3g.tarul.cn/Article/details/gcadsvfrh.sHtML

structuredClone(obj)
来源：http://mobile.epnwcf.com/Article/details/gedvcxjbi.sHtML

[U93] JS：模板字符串
来源：http://read.share.sjlbkw.cn/Article/details/gsilqbnrl.sHtML

`共 ${n} 条`
来源：http://www.blog.yfazqb.com/Article/details/ghdkmqncn.sHtML

[U94] JS：箭头函数
来源：http://blog.tarul.cn/Article/details/gakdittdv.sHtML

const double = x => x * 2;
来源：http://m.share.bbcook.cn/Article/details/ghyxwvcst.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fktsv.cn/Article/details/gsihorezz.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.bbcook.cn/Article/details/gfpdpyary.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.epnwcf.com/Article/details/gljutmwnz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.epnwcf.com/Article/details/gleboqtyk.sHtML

[U97] JS：并发请求
来源：http://wap.epnwcf.com/Article/details/gwhswoziw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.tarul.cn/Article/details/gthagrlkc.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.yfazqb.com/Article/details/gdqrpovie.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.tarul.cn/Article/details/gusgsxsvh.sHtML

[U99] JS：事件监听
来源：http://mobile.sjlbkw.cn/Article/details/gxvtjymru.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.tarul.cn/Article/details/gpwbwqotp.sHtML

[U100] JS：DOM 查询
来源：http://www.share.epnwcf.com/Article/details/gykuaijjd.sHtML

document.querySelector(".item")
来源：http://3g.bbcook.cn/Article/details/guudwvqqq.sHtML

[U101] JS：classList 操作
来源：http://read.share.fktsv.cn/Article/details/gwrjpcema.sHtML

el.classList.toggle("active")
来源：http://www.blog.fktsv.cn/Article/details/gagpojgjc.sHtML

[U102] JS：本地存储
来源：http://baike.bbcook.cn/Article/details/glknkjmce.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.tarul.cn/Article/details/gxmaocapw.sHtML

[U103] JS：定时器
来源：http://blog.sjlbkw.cn/Article/details/golvswcvo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.yfazqb.com/Article/details/gwhzcqaaq.sHtML

[U104] JS：防抖
来源：http://www.blog.vehdjk.com/Article/details/gprtaoevy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.vehdjk.com/Article/details/gtovtrgsl.sHtML

[U105] JS：节流
来源：http://baike.bbcook.cn/Article/details/gtxahnhrc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.sjlbkw.cn/Article/details/gpvzlwlvf.sHtML

[U106] JS：日期格式化
来源：http://wap.fktsv.cn/Article/details/gjabsclmt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.bbcook.cn/Article/details/gdlclatya.sHtML

[U107] JS：数字千分位
来源：http://m.share.tarul.cn/Article/details/gwgrrlmqc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.vehdjk.com/Article/details/gnhhlmayi.sHtML

[U108] JS：随机整数
来源：http://read.share.epnwcf.com/Article/details/guxwpnyyp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.vehdjk.com/Article/details/gwyskxish.sHtML

[U109] JS：数组分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gehxlqqfo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.sjlbkw.cn/Article/details/gqqvfrtse.sHtML

[U110] JS：数组分块
来源：http://www.m.share.tarul.cn/Article/details/goirogmug.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.tarul.cn/Article/details/gzjsscxpy.sHtML

[U111] JS：对象转 Map
来源：http://wap.fktsv.cn/Article/details/gmhmnmcai.sHtML

new Map(Object.entries(obj))
来源：http://www.share.yfazqb.com/Article/details/gmwqibinx.sHtML

[U112] JS：字符串补位
来源：http://baike.sjlbkw.cn/Article/details/gighzlxzu.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fktsv.cn/Article/details/gxxdsetar.sHtML

[U113] JS：正则替换全部
来源：http://www.share.vehdjk.com/Article/details/gxjehyokp.sHtML

s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gztelvkne.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.tarul.cn/Article/details/gwyfyrlbb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.tarul.cn/Article/details/gdsxwnnaj.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.vehdjk.com/Article/details/gmfjrjrnk.sHtML

crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gjxrzafxn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.bbcook.cn/Article/details/ggxbspmid.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.sjlbkw.cn/Article/details/gdlzxojsa.sHtML

[U117] JS：单元测试
来源：http://baike.sjlbkw.cn/Article/details/gqwnbfzzj.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.sjlbkw.cn/Article/details/grjixkmnr.sHtML

[U118] JS：开发服务器
来源：http://blog.sjlbkw.cn/Article/details/gsnjdidad.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fktsv.cn/Article/details/gdygtwvlm.sHtML

[U119] JS：生产构建
来源：http://read.share.vehdjk.com/Article/details/gsmajhdnd.sHtML

npx vite build
来源：http://wap.epnwcf.com/Article/details/gfuxbiarj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.tarul.cn/Article/details/grqbqitlt.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fktsv.cn/Article/details/gtiwnrhvo.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/godrkrcwv.sHtML

统计汇总
来源：http://www.blog.fktsv.cn/Article/details/gfgwqnxhf.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gdrvyuqto.sHtML

按语言统计（条）：
来源：http://3g.sjlbkw.cn/Article/details/glgdyapyi.sHtML

Python ......... 252
来源：http://baike.bbcook.cn/Article/details/gtyxawzid.sHtML

PHP ............ 252
来源：http://read.share.bbcook.cn/Article/details/grudnlxty.sHtML

JavaScript ..... 252
来源：http://www.blog.tarul.cn/Article/details/grfptdvrv.sHtML

TypeScript ..... 212
来源：http://wap.bbcook.cn/Article/details/gydzvmmxo.sHtML

Java ........... 212
来源：http://baike.yfazqb.com/Article/details/gcbempfmb.sHtML

Go ............. 212
来源：http://www.share.vehdjk.com/Article/details/gxqgoxqzx.sHtML

Ruby ........... 212
来源：http://www.share.sjlbkw.cn/Article/details/gpnpjauuq.sHtML

C# ............. 212
来源：http://www.m.share.epnwcf.com/Article/details/gjcvwnlbi.sHtML

C .............. 30
来源：http://m.share.sjlbkw.cn/Article/details/gllvpitwv.sHtML

C++ ............ 30
来源：http://read.share.epnwcf.com/Article/details/gzfggekou.sHtML

SQL ............ 90
来源：http://mobile.yfazqb.com/Article/details/gkevswvus.sHtML

Bash ........... 80
来源：http://3g.vehdjk.com/Article/details/ggjznjspc.sHtML

Kotlin ......... 15
来源：http://blog.yfazqb.com/Article/details/gzoidrpab.sHtML

Swift .......... 15
来源：http://blog.bbcook.cn/Article/details/gmezzdagn.sHtML

Lua ............ 10
来源：http://read.share.yfazqb.com/Article/details/gxfxnjbkw.sHtML

Perl ........... 10
来源：http://www.m.share.fktsv.cn/Article/details/gplnqalew.sHtML

Scala .......... 10
来源：http://3g.fktsv.cn/Article/details/giwgcqswb.sHtML

------------------------------------
来源：http://read.share.yfazqb.com/Article/details/gkwoycodu.sHtML

合计 ........... 2106 条
来源：http://read.share.vehdjk.com/Article/details/gfrdcgxsg.sHtML

按章节统计：
来源：http://baike.fktsv.cn/Article/details/gobtaqean.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.bbcook.cn/Article/details/golpuirhe.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.vehdjk.com/Article/details/guqgxyxvl.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fktsv.cn/Article/details/gmqlzriks.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.tarul.cn/Article/details/gtbdypesl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.sjlbkw.cn/Article/details/gliogqltr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.epnwcf.com/Article/details/gzovewfxx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fktsv.cn/Article/details/gazyjkuua.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.tarul.cn/Article/details/gtczrspfu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fktsv.cn/Article/details/gjwvntxgo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fktsv.cn/Article/details/gwyoscxej.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.sjlbkw.cn/Article/details/gusrvkanc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.tarul.cn/Article/details/gpksvjfxq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gtwqsazyo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.bbcook.cn/Article/details/gfgbxdxyh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.epnwcf.com/Article/details/gtsafmjmk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/gwabbcrij.sHtML

Q SQL 专题                              90
来源：http://blog.yfazqb.com/Article/details/gnbnwvcut.sHtML

R Bash 专题                             80
来源：http://baike.sjlbkw.cn/Article/details/gkejpoqhp.sHtML

S C / C++ 专题                          60
来源：http://baike.epnwcf.com/Article/details/grirxqxpy.sHtML

T 其他语言补充                          60
来源：http://baike.vehdjk.com/Article/details/gnecgsbvq.sHtML


<!-- 参考信息 -->