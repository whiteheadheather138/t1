代发 wailian999

[U01] Py：创建虚拟环境
来源：http://m.share.epnwcf.com/Article/details/gvpghdtxi.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://blog.vehdjk.com/Article/details/ghtgprdzw.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.epnwcf.com/Article/details/gqzebivxl.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mobile.yfazqb.com/Article/details/gflagfciq.sHtML

[U03] Py：加载 .env 配置
来源：http://3g.fktsv.cn/Article/details/gdwavkswb.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://3g.tarul.cn/Article/details/gbhiqvaye.sHtML

[U04] Py：变量调试打印
来源：http://www.share.sjlbkw.cn/Article/details/ggfdszzsa.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.yfazqb.com/Article/details/gwdwtzrrz.sHtML

[U05] Py：列表去重且保序
来源：http://baike.yfazqb.com/Article/details/gjfwqppvr.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.vehdjk.com/Article/details/gqsegplty.sHtML

[U06] Py：合并两个字典
来源：http://3g.tarul.cn/Article/details/giimqnmvk.sHtML

{**a, **b}
来源：http://baike.yfazqb.com/Article/details/gvmpasqln.sHtML

[U07] Py：反转字典键值
来源：http://read.share.vehdjk.com/Article/details/gghfbkunj.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.tarul.cn/Article/details/gszowgoam.sHtML

[U08] Py：展平二维列表
来源：http://blog.epnwcf.com/Article/details/gjohrcoel.sHtML

[y for x in nested for y in x]
来源：http://www.m.share.yfazqb.com/Article/details/gvfwabjxb.sHtML

[U09] Py：字典取最大值的键
来源：http://baike.yfazqb.com/Article/details/gfhbxjpro.sHtML

max(d, key=d.get)
来源：http://mobile.bbcook.cn/Article/details/grbmyqzqf.sHtML

[U10] Py：按值排序字典
来源：http://3g.yfazqb.com/Article/details/gduebnkif.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://3g.fktsv.cn/Article/details/ghahboljm.sHtML

[U11] Py：生成器表达式
来源：http://blog.epnwcf.com/Article/details/ggrrsvszz.sHtML

(x * 2 for x in arr)
来源：http://m.share.vehdjk.com/Article/details/gvyfxzgtk.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.vehdjk.com/Article/details/gsmwgmntz.sHtML

Counter(arr).most_common(3)
来源：http://mobile.epnwcf.com/Article/details/gfbjuvyqg.sHtML

[U13] Py：固定长度队列
来源：http://mobile.fktsv.cn/Article/details/gmxslujsv.sHtML

deque(maxlen=10)
来源：http://baike.bbcook.cn/Article/details/gfihfhycv.sHtML

[U14] Py：分组收集到列表
来源：http://wap.epnwcf.com/Article/details/gefvmxqyw.sHtML

defaultdict(list)
来源：http://mobile.bbcook.cn/Article/details/gvsjvjyts.sHtML

[U15] Py：高精度计时
来源：http://read.share.bbcook.cn/Article/details/gbnxcgujl.sHtML

t = time.perf_counter()
来源：http://mobile.fktsv.cn/Article/details/gbnoqpgah.sHtML

[U16] Py：命令行参数解析
来源：http://baike.yfazqb.com/Article/details/ghcyzhraq.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.m.share.vehdjk.com/Article/details/gbxrlnggh.sHtML

[U17] Py：初始化日志
来源：http://www.share.epnwcf.com/Article/details/gujirtmsw.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://read.share.sjlbkw.cn/Article/details/gouznshct.sHtML

[U18] Py：预编译正则
来源：http://m.share.sjlbkw.cn/Article/details/gprlastnn.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.tarul.cn/Article/details/gvlsicosd.sHtML

[U19] Py：正则替换带回调
来源：http://mobile.fktsv.cn/Article/details/gpxdlddur.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.tarul.cn/Article/details/geryqzvar.sHtML

[U20] Py：缓存函数结果
来源：http://3g.bbcook.cn/Article/details/gjbokzbtg.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.tarul.cn/Article/details/gtkurafkx.sHtML

[U21] Py：自定义上下文管理器
来源：http://m.share.bbcook.cn/Article/details/gsahqfoia.sHtML

@contextlib.contextmanager
来源：http://www.m.share.epnwcf.com/Article/details/gxestfkjf.sHtML

[U22] Py：矩阵转置
来源：http://blog.tarul.cn/Article/details/gqaswzpvs.sHtML

list(zip(*m))
来源：http://www.share.epnwcf.com/Article/details/ggdpdjpds.sHtML

[U23] Py：分块读取大文件
来源：http://wap.tarul.cn/Article/details/gqyxxoydt.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.yfazqb.com/Article/details/ggykmqqqp.sHtML

[U24] Py：路径操作
来源：http://wap.bbcook.cn/Article/details/gxazkxlur.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://read.share.fktsv.cn/Article/details/ghyaasbrc.sHtML

[U25] Py：CSV 按字典读
来源：http://blog.fktsv.cn/Article/details/gjukdlvkx.sHtML

csv.DictReader(f)
来源：http://m.share.tarul.cn/Article/details/gpanwpcxp.sHtML

[U26] Py：并发下载
来源：http://m.share.yfazqb.com/Article/details/gqpyzmzmb.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.share.tarul.cn/Article/details/gfqhxklbd.sHtML

[U27] Py：异步 HTTP
来源：http://mobile.tarul.cn/Article/details/gtlirakum.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://baike.bbcook.cn/Article/details/ggkfqevip.sHtML

[U28] Py：类型别名
来源：http://mobile.yfazqb.com/Article/details/gjrflnbxq.sHtML

UserId = int
来源：http://baike.bbcook.cn/Article/details/gfumxybjw.sHtML

[U29] Py：属性校验
来源：http://www.blog.fktsv.cn/Article/details/gebwvhnub.sHtML

@property 与 @x.setter 配合
来源：http://www.share.vehdjk.com/Article/details/gopfqlvuc.sHtML

[U30] Py：数据类
来源：http://blog.bbcook.cn/Article/details/ghdvjwreq.sHtML

@dataclass(slots=True)
来源：http://www.share.yfazqb.com/Article/details/gggizwfwm.sHtML

[U31] Py：单测
来源：http://wap.yfazqb.com/Article/details/ggbecwkqu.sHtML

python -m pytest -q
来源：http://3g.vehdjk.com/Article/details/givkxdgnx.sHtML

[U32] Py：代码格式化
来源：http://www.blog.fktsv.cn/Article/details/ghuatxxvy.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.yfazqb.com/Article/details/gayqjjctf.sHtML

[U33] Py：打包发布
来源：http://3g.fktsv.cn/Article/details/gaklsydmq.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://read.share.tarul.cn/Article/details/ghdptpnam.sHtML

[U34] Py：判断编码
来源：http://blog.tarul.cn/Article/details/gphuasmbw.sHtML

chardet.detect(raw)
来源：http://blog.fktsv.cn/Article/details/grkrqwfku.sHtML

[U35] Py：发送邮件
来源：http://mobile.epnwcf.com/Article/details/gqulwovzn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.blog.vehdjk.com/Article/details/gitbwmyia.sHtML

[U36] Py：定时任务
来源：http://m.share.tarul.cn/Article/details/gvbelvzvj.sHtML

schedule.every(10).minutes.do(job)
来源：http://www.m.share.epnwcf.com/Article/details/gomycxfmo.sHtML

[U37] Py：读写 Excel
来源：http://mobile.sjlbkw.cn/Article/details/gcnvzugby.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://m.share.sjlbkw.cn/Article/details/grigrzolw.sHtML

[U38] Py：获取脚本所在目录
来源：http://wap.tarul.cn/Article/details/gvkjsnwtf.sHtML

Path(__file__).resolve().parent
来源：http://3g.fktsv.cn/Article/details/gilwsytyu.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.tarul.cn/Article/details/gzpoirclb.sHtML

sys.stdout.isatty()
来源：http://mobile.fktsv.cn/Article/details/gooozwurd.sHtML

[U40] Py：打印到标准错误
来源：http://mobile.epnwcf.com/Article/details/ggfdcdkru.sHtML

print("err", file=sys.stderr)
来源：http://blog.bbcook.cn/Article/details/grpqusjun.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.share.yfazqb.com/Article/details/gsxmajyqu.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://mobile.bbcook.cn/Article/details/gboczplhv.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.epnwcf.com/Article/details/gsyvpakcy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.bbcook.cn/Article/details/guxspdxou.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fktsv.cn/Article/details/ghpaperzv.sHtML

namespace App\Http;
来源：http://www.blog.bbcook.cn/Article/details/gslheywsp.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.vehdjk.com/Article/details/gwdxkunac.sHtML

declare(strict_types=1);
来源：http://read.share.tarul.cn/Article/details/gyosrwjnh.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.epnwcf.com/Article/details/gpluqkzil.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.yfazqb.com/Article/details/guparnodb.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.epnwcf.com/Article/details/ganjfaslo.sHtML

?string $name = null
来源：http://read.share.yfazqb.com/Article/details/getcpvonw.sHtML

[U47] PHP：联合类型
来源：http://baike.bbcook.cn/Article/details/gslyrbskt.sHtML

int|string $id
来源：http://read.share.vehdjk.com/Article/details/geutbcjxa.sHtML

[U48] PHP：纯枚举
来源：http://3g.bbcook.cn/Article/details/gadtibncf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.yfazqb.com/Article/details/gpsohmjzv.sHtML

[U49] PHP：只读属性
来源：http://wap.yfazqb.com/Article/details/gixwepapm.sHtML

public readonly string $name
来源：http://www.m.share.yfazqb.com/Article/details/geyvvkkoi.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.epnwcf.com/Article/details/gwjyyztnw.sHtML

public function __construct(private int $id) {}
来源：http://www.share.sjlbkw.cn/Article/details/giiumzgld.sHtML

[U51] PHP：数组解构
来源：http://mobile.tarul.cn/Article/details/gkxqkathg.sHtML

[$a, $b] = $arr;
来源：http://baike.sjlbkw.cn/Article/details/gdjzwwcla.sHtML

[U52] PHP：箭头函数
来源：http://wap.yfazqb.com/Article/details/gdifpopvk.sHtML

$double = fn($x) => $x * 2;
来源：http://www.share.fktsv.cn/Article/details/gxzfmygxq.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.yfazqb.com/Article/details/gbnloowxb.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fktsv.cn/Article/details/gamnhufao.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fktsv.cn/Article/details/gimikqaso.sHtML

$obj?->method()
来源：http://www.share.yfazqb.com/Article/details/gpcbideml.sHtML

[U55] PHP：match 表达式
来源：http://www.share.sjlbkw.cn/Article/details/grfcjwnzf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.tarul.cn/Article/details/gwnjtxifl.sHtML

[U56] PHP：命名参数
来源：http://www.blog.yfazqb.com/Article/details/guaumzker.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.vehdjk.com/Article/details/glleaedfs.sHtML

[U57] PHP：字符串插值
来源：http://m.share.sjlbkw.cn/Article/details/geunsffqh.sHtML

"值: {$a}"
来源：http://3g.sjlbkw.cn/Article/details/gtscpoozf.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.epnwcf.com/Article/details/gwojfaoeq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.epnwcf.com/Article/details/gxebqafel.sHtML

[U59] PHP：自定义排序
来源：http://wap.bbcook.cn/Article/details/gkxdhmnnp.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fktsv.cn/Article/details/gsbounevy.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.sjlbkw.cn/Article/details/gbefxhmpw.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.vehdjk.com/Article/details/gnizzhled.sHtML

[U61] PHP：正则
来源：http://www.blog.epnwcf.com/Article/details/glxwsbkrw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.tarul.cn/Article/details/gtnrqwjgy.sHtML

[U62] PHP：日期对象
来源：http://www.share.tarul.cn/Article/details/gfyfvchjv.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.vehdjk.com/Article/details/gcqzdinsq.sHtML

[U63] PHP：文件读写
来源：http://m.share.epnwcf.com/Article/details/gbvnyahsk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.bbcook.cn/Article/details/gvujhwkzx.sHtML

[U64] PHP：目录遍历
来源：http://www.share.bbcook.cn/Article/details/gvpmgvtju.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.epnwcf.com/Article/details/gsbbzvcgs.sHtML

[U65] PHP：会话
来源：http://read.share.vehdjk.com/Article/details/geoewqhhe.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.vehdjk.com/Article/details/gfqbhjvyy.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.epnwcf.com/Article/details/gfuojgitc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.tarul.cn/Article/details/gavfltvta.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.bbcook.cn/Article/details/gtsglbugb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fktsv.cn/Article/details/gzwkntsxi.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.tarul.cn/Article/details/gtfhzozba.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.bbcook.cn/Article/details/gvdbqrhdx.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.vehdjk.com/Article/details/gdgnuosea.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.bbcook.cn/Article/details/gafcqdipb.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.bbcook.cn/Article/details/gvxdewgus.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.tarul.cn/Article/details/ggzgjiymg.sHtML

[U71] PHP：抛出异常
来源：http://www.share.vehdjk.com/Article/details/gdfjlqgic.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.epnwcf.com/Article/details/gwveakalw.sHtML

[U72] PHP：写错误日志
来源：http://www.share.sjlbkw.cn/Article/details/gghtqrzpu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.tarul.cn/Article/details/gutvvfvbu.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fktsv.cn/Article/details/gzsnmwwff.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.vehdjk.com/Article/details/gxxyslyzp.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.epnwcf.com/Article/details/gkpldcwbm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.tarul.cn/Article/details/gienmuaho.sHtML

[U75] PHP：依赖注入
来源：http://wap.yfazqb.com/Article/details/gnpgmynyd.sHtML

composer require psr/container
来源：http://3g.epnwcf.com/Article/details/grigrntkn.sHtML

[U76] PHP：简单路由
来源：http://baike.tarul.cn/Article/details/guqgcxaev.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.sjlbkw.cn/Article/details/glxrrwayl.sHtML

[U77] PHP：模板渲染
来源：http://blog.epnwcf.com/Article/details/gzxawcook.sHtML

composer require twig/twig
来源：http://m.share.yfazqb.com/Article/details/gslghwykz.sHtML

[U78] PHP：单元测试
来源：http://m.share.bbcook.cn/Article/details/ghkkdcfsp.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fktsv.cn/Article/details/gdzqowejw.sHtML

[U79] PHP：静态分析
来源：http://wap.sjlbkw.cn/Article/details/ggjavdtwh.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.epnwcf.com/Article/details/gmofqdwpb.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.sjlbkw.cn/Article/details/ggajswhww.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.epnwcf.com/Article/details/giabwghot.sHtML

[U81] JS：初始化项目
来源：http://www.blog.bbcook.cn/Article/details/gvumltzqo.sHtML

npm init -y;  npm i express
来源：http://www.share.vehdjk.com/Article/details/gvfjcflqv.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fktsv.cn/Article/details/gkgquslky.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fktsv.cn/Article/details/gorcygurv.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.vehdjk.com/Article/details/gpchynojf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.vehdjk.com/Article/details/gvvspvtzv.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.bbcook.cn/Article/details/grwwfqhdq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.sjlbkw.cn/Article/details/gdrmvnekx.sHtML

[U85] JS：可选链
来源：http://mobile.tarul.cn/Article/details/gfhetasyw.sHtML

a?.b?.c
来源：http://wap.vehdjk.com/Article/details/gwngyoobq.sHtML

[U86] JS：空值合并
来源：http://m.share.yfazqb.com/Article/details/gkqrpnjmi.sHtML

a ?? b
来源：http://www.m.share.fktsv.cn/Article/details/gvktxhklm.sHtML

[U87] JS：解构默认值
来源：http://wap.sjlbkw.cn/Article/details/gqscoyfqv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.vehdjk.com/Article/details/gcekvzvei.sHtML

[U88] JS：对象展开合并
来源：http://blog.fktsv.cn/Article/details/gbxtoqxna.sHtML

{ ...a, ...b }
来源：http://read.share.fktsv.cn/Article/details/glcemfjao.sHtML

[U89] JS：数组去重
来源：http://www.m.share.tarul.cn/Article/details/gkvekbnke.sHtML

[...new Set(arr)]
来源：http://read.share.epnwcf.com/Article/details/gwdqjnhpc.sHtML

[U90] JS：数字数组排序
来源：http://3g.fktsv.cn/Article/details/giyhpxlim.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/gnvvkfpna.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.bbcook.cn/Article/details/gxepixgmu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.sjlbkw.cn/Article/details/gqgtmcquk.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fktsv.cn/Article/details/goihvalju.sHtML

structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/gcqfzcfik.sHtML

[U93] JS：模板字符串
来源：http://mobile.fktsv.cn/Article/details/gxdaezzvs.sHtML

`共 ${n} 条`
来源：http://www.blog.yfazqb.com/Article/details/gdcfnehhb.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fktsv.cn/Article/details/gahwftxyv.sHtML

const double = x => x * 2;
来源：http://3g.fktsv.cn/Article/details/gqfcehruq.sHtML

[U95] JS：Promise 包装
来源：http://www.share.sjlbkw.cn/Article/details/gwtpahudg.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.yfazqb.com/Article/details/gpsbbnlpg.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.bbcook.cn/Article/details/gjgismtzi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.epnwcf.com/Article/details/gpxtibonc.sHtML

[U97] JS：并发请求
来源：http://mobile.bbcook.cn/Article/details/ghkgvjgdr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.epnwcf.com/Article/details/gybpmoxpm.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.vehdjk.com/Article/details/gcukeafww.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.tarul.cn/Article/details/gjfnlijaz.sHtML

[U99] JS：事件监听
来源：http://baike.bbcook.cn/Article/details/gaxbmcpgk.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fktsv.cn/Article/details/gaurkmeyl.sHtML

[U100] JS：DOM 查询
来源：http://wap.fktsv.cn/Article/details/gxrtptzni.sHtML

document.querySelector(".item")
来源：http://3g.vehdjk.com/Article/details/gajxvlyzq.sHtML

[U101] JS：classList 操作
来源：http://read.share.fktsv.cn/Article/details/gjbxbowox.sHtML

el.classList.toggle("active")
来源：http://www.blog.sjlbkw.cn/Article/details/gmsjpvufr.sHtML

[U102] JS：本地存储
来源：http://mobile.bbcook.cn/Article/details/gwpiiwctt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.yfazqb.com/Article/details/goowopopt.sHtML

[U103] JS：定时器
来源：http://m.share.fktsv.cn/Article/details/gskncixol.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.vehdjk.com/Article/details/gefxmpysn.sHtML

[U104] JS：防抖
来源：http://m.share.yfazqb.com/Article/details/gknyuxpfl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.epnwcf.com/Article/details/gsmahsoji.sHtML

[U105] JS：节流
来源：http://baike.sjlbkw.cn/Article/details/gksryhogi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fktsv.cn/Article/details/gbdajvinr.sHtML

[U106] JS：日期格式化
来源：http://3g.sjlbkw.cn/Article/details/gycljgqbh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.tarul.cn/Article/details/ghbpmvwur.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.vehdjk.com/Article/details/gdmoxrdea.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.tarul.cn/Article/details/gaupvajdi.sHtML

[U108] JS：随机整数
来源：http://www.m.share.yfazqb.com/Article/details/gasbfqdck.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.vehdjk.com/Article/details/gpzvxkidx.sHtML

[U109] JS：数组分组
来源：http://www.blog.tarul.cn/Article/details/gjeuxoufl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.sjlbkw.cn/Article/details/gmckajdwr.sHtML

[U110] JS：数组分块
来源：http://baike.epnwcf.com/Article/details/gqszebatj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.yfazqb.com/Article/details/gyqzlkixu.sHtML

[U111] JS：对象转 Map
来源：http://blog.tarul.cn/Article/details/ghquprrlq.sHtML

new Map(Object.entries(obj))
来源：http://wap.yfazqb.com/Article/details/gxfdlmoml.sHtML

[U112] JS：字符串补位
来源：http://baike.sjlbkw.cn/Article/details/gyxiwuhis.sHtML

"7".padStart(3, "0")
来源：http://m.share.fktsv.cn/Article/details/gycicsike.sHtML

[U113] JS：正则替换全部
来源：http://m.share.sjlbkw.cn/Article/details/gwvlwzlyl.sHtML

s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/gldijprzr.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.epnwcf.com/Article/details/glgoirtkd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.yfazqb.com/Article/details/gvukgjxor.sHtML

[U115] JS：生成 UUID
来源：http://m.share.bbcook.cn/Article/details/gfuzdqiyq.sHtML

crypto.randomUUID()
来源：http://mobile.yfazqb.com/Article/details/gwyzgifwe.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fktsv.cn/Article/details/gstnagpca.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.yfazqb.com/Article/details/ginftfday.sHtML

[U117] JS：单元测试
来源：http://m.share.sjlbkw.cn/Article/details/gqgfohdsf.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.vehdjk.com/Article/details/grtbthyhr.sHtML

[U118] JS：开发服务器
来源：http://m.share.yfazqb.com/Article/details/grnbroclo.sHtML

npm i -D vite;  npx vite
来源：http://wap.sjlbkw.cn/Article/details/gtuemfcrs.sHtML

[U119] JS：生产构建
来源：http://wap.vehdjk.com/Article/details/gpivonsuq.sHtML

npx vite build
来源：http://baike.tarul.cn/Article/details/gntqtmrgj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.vehdjk.com/Article/details/gkcjbsowg.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.bbcook.cn/Article/details/goqsgqxek.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gaktlgpcp.sHtML

统计汇总
来源：http://baike.fktsv.cn/Article/details/gxddicwvj.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gtcyjczxu.sHtML

按语言统计（条）：
来源：http://www.share.epnwcf.com/Article/details/gwgsrzsny.sHtML

Python ......... 252
来源：http://baike.epnwcf.com/Article/details/gjavzheir.sHtML

PHP ............ 252
来源：http://blog.yfazqb.com/Article/details/guiekjkny.sHtML

JavaScript ..... 252
来源：http://blog.tarul.cn/Article/details/gkuisviat.sHtML

TypeScript ..... 212
来源：http://read.share.bbcook.cn/Article/details/glgrkhjfy.sHtML

Java ........... 212
来源：http://3g.fktsv.cn/Article/details/gqchcazzn.sHtML

Go ............. 212
来源：http://3g.vehdjk.com/Article/details/grdjobbav.sHtML

Ruby ........... 212
来源：http://blog.epnwcf.com/Article/details/gcnfrpimv.sHtML

C# ............. 212
来源：http://read.share.fktsv.cn/Article/details/gaoytrgwx.sHtML

C .............. 30
来源：http://read.share.epnwcf.com/Article/details/gsoukghhs.sHtML

C++ ............ 30
来源：http://mobile.tarul.cn/Article/details/gwjryurhz.sHtML

SQL ............ 90
来源：http://read.share.epnwcf.com/Article/details/gmfusmbjh.sHtML

Bash ........... 80
来源：http://mobile.bbcook.cn/Article/details/gvwpyvpny.sHtML

Kotlin ......... 15
来源：http://blog.epnwcf.com/Article/details/gsibglsjf.sHtML

Swift .......... 15
来源：http://read.share.tarul.cn/Article/details/gkmgokyyj.sHtML

Lua ............ 10
来源：http://read.share.tarul.cn/Article/details/gybqqcoln.sHtML

Perl ........... 10
来源：http://www.m.share.vehdjk.com/Article/details/gxkhntncc.sHtML

Scala .......... 10
来源：http://www.blog.sjlbkw.cn/Article/details/giwzyfsmm.sHtML

------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gphsuqbpx.sHtML

合计 ........... 2106 条
来源：http://read.share.vehdjk.com/Article/details/gsuatzgak.sHtML

按章节统计：
来源：http://www.share.epnwcf.com/Article/details/gvhtvuiug.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.vehdjk.com/Article/details/gvxllqztt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.epnwcf.com/Article/details/gtobptxfr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.epnwcf.com/Article/details/ggmzzxkun.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.vehdjk.com/Article/details/gzjmeykym.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.sjlbkw.cn/Article/details/ghmgpeeki.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.bbcook.cn/Article/details/glxfbixqy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.tarul.cn/Article/details/gbdgstebi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.bbcook.cn/Article/details/gsjhrlasm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/gpaeqneuu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.bbcook.cn/Article/details/gwawqovpv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/grxyyxtgo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.sjlbkw.cn/Article/details/gjuafpbef.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.yfazqb.com/Article/details/gwrwtdmrk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.tarul.cn/Article/details/gkgbkvapa.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.tarul.cn/Article/details/gomwqfruk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/gplgtdrtj.sHtML

Q SQL 专题                              90
来源：http://blog.bbcook.cn/Article/details/gsghpnvgq.sHtML

R Bash 专题                             80
来源：http://blog.epnwcf.com/Article/details/gnjohsmex.sHtML

S C / C++ 专题                          60
来源：http://www.blog.sjlbkw.cn/Article/details/gkvqyxrbi.sHtML

T 其他语言补充                          60
来源：http://baike.tarul.cn/Article/details/ghtsrjgtc.sHtML

U 高频实用片段                         120
来源：http://read.share.fktsv.cn/Article/details/gxcxpiuaz.sHtML

------------------------------------
来源：http://read.share.vehdjk.com/Article/details/glpsfqoun.sHtML

合计                                  2106 条
来源：http://read.share.vehdjk.com/Article/details/gmslnoxhk.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gtzcxweum.sHtML

使用提醒
来源：http://www.blog.tarul.cn/Article/details/gxbzqzgjr.sHtML

--------------------------------------------------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/gzsgxdzgn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.epnwcf.com/Article/details/gbuhjijmd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.sjlbkw.cn/Article/details/gyjpzektc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.tarul.cn/Article/details/gkwcyzyxi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.epnwcf.com/Article/details/gritzwyss.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.vehdjk.com/Article/details/giesafvpg.sHtML

—— 文件结束 ——
来源：http://www.m.share.sjlbkw.cn/Article/details/gsinfpvij.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gtrunlnji.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.epnwcf.com/Article/details/gyvuwuqhg.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.vehdjk.com/Article/details/gqvnmycwp.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gklpjcrkp.sHtML


<!-- 参考信息 -->