代发 wailian999

[U01] Py：创建虚拟环境
来源：http://m.share.fktsv.cn/Article/details/gilwdfpau.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://mobile.sjlbkw.cn/Article/details/gnqqkxjba.sHtML

[U02] Py：导出 / 安装依赖
来源：http://mobile.vehdjk.com/Article/details/gkrxpexxw.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://read.share.vehdjk.com/Article/details/gwjhwvlgi.sHtML

[U03] Py：加载 .env 配置
来源：http://www.m.share.vehdjk.com/Article/details/gijtyainh.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://m.share.vehdjk.com/Article/details/gwpzppjxs.sHtML

[U04] Py：变量调试打印
来源：http://blog.epnwcf.com/Article/details/gteskbnta.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://blog.vehdjk.com/Article/details/gaqmqgmdf.sHtML

[U05] Py：列表去重且保序
来源：http://baike.bbcook.cn/Article/details/ggcspnhow.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.sjlbkw.cn/Article/details/gkztwiahl.sHtML

[U06] Py：合并两个字典
来源：http://baike.epnwcf.com/Article/details/gedmopcud.sHtML

{**a, **b}
来源：http://www.m.share.epnwcf.com/Article/details/gcvennmpo.sHtML

[U07] Py：反转字典键值
来源：http://read.share.yfazqb.com/Article/details/ghvgmszzs.sHtML

{v: k for k, v in d.items()}
来源：http://mobile.vehdjk.com/Article/details/gcjfkvdal.sHtML

[U08] Py：展平二维列表
来源：http://baike.vehdjk.com/Article/details/gutspehuy.sHtML

[y for x in nested for y in x]
来源：http://mobile.bbcook.cn/Article/details/gdmyrcaai.sHtML

[U09] Py：字典取最大值的键
来源：http://wap.yfazqb.com/Article/details/gfavyqttv.sHtML

max(d, key=d.get)
来源：http://3g.bbcook.cn/Article/details/gpwdluanm.sHtML

[U10] Py：按值排序字典
来源：http://3g.tarul.cn/Article/details/gjlmsfrzq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.vehdjk.com/Article/details/ggszosjjp.sHtML

[U11] Py：生成器表达式
来源：http://www.share.epnwcf.com/Article/details/gwhabznpx.sHtML

(x * 2 for x in arr)
来源：http://www.m.share.yfazqb.com/Article/details/ghajjgpjr.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://mobile.sjlbkw.cn/Article/details/gieucsavy.sHtML

Counter(arr).most_common(3)
来源：http://www.m.share.yfazqb.com/Article/details/guwrycwwr.sHtML

[U13] Py：固定长度队列
来源：http://mobile.tarul.cn/Article/details/gwodpiiij.sHtML

deque(maxlen=10)
来源：http://wap.sjlbkw.cn/Article/details/gtcjubknx.sHtML

[U14] Py：分组收集到列表
来源：http://blog.epnwcf.com/Article/details/gnbhaijpz.sHtML

defaultdict(list)
来源：http://blog.tarul.cn/Article/details/gmjrojsom.sHtML

[U15] Py：高精度计时
来源：http://baike.yfazqb.com/Article/details/gddwdvxoa.sHtML

t = time.perf_counter()
来源：http://m.share.vehdjk.com/Article/details/gzozhyace.sHtML

[U16] Py：命令行参数解析
来源：http://wap.vehdjk.com/Article/details/gyqasnxki.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.yfazqb.com/Article/details/gykdkmcas.sHtML

[U17] Py：初始化日志
来源：http://wap.vehdjk.com/Article/details/gkotzlosn.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://baike.bbcook.cn/Article/details/gohrutdma.sHtML

[U18] Py：预编译正则
来源：http://baike.vehdjk.com/Article/details/gwdpezsbn.sHtML

pat = re.compile(r"\d+")
来源：http://mobile.vehdjk.com/Article/details/gingkesfa.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.yfazqb.com/Article/details/gdchefcdp.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.epnwcf.com/Article/details/gprxohmah.sHtML

[U20] Py：缓存函数结果
来源：http://baike.fktsv.cn/Article/details/ghbknyygo.sHtML

@functools.lru_cache(maxsize=None)
来源：http://3g.yfazqb.com/Article/details/gdlgcqxqq.sHtML

[U21] Py：自定义上下文管理器
来源：http://baike.tarul.cn/Article/details/grxunyiwh.sHtML

@contextlib.contextmanager
来源：http://3g.bbcook.cn/Article/details/gzzxaynfv.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.yfazqb.com/Article/details/gfcrncmth.sHtML

list(zip(*m))
来源：http://mobile.bbcook.cn/Article/details/geldliboi.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.bbcook.cn/Article/details/gdlfzqilx.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://read.share.vehdjk.com/Article/details/gzegyocms.sHtML

[U24] Py：路径操作
来源：http://mobile.tarul.cn/Article/details/gytqjbndf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://baike.tarul.cn/Article/details/gqvfthsrt.sHtML

[U25] Py：CSV 按字典读
来源：http://www.blog.sjlbkw.cn/Article/details/grubifpcr.sHtML

csv.DictReader(f)
来源：http://www.m.share.vehdjk.com/Article/details/gbhgbdnku.sHtML

[U26] Py：并发下载
来源：http://www.blog.bbcook.cn/Article/details/gflssvnjs.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://baike.yfazqb.com/Article/details/gzlrbkfgh.sHtML

[U27] Py：异步 HTTP
来源：http://wap.yfazqb.com/Article/details/gsxrrcdov.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://www.blog.tarul.cn/Article/details/glvtufonh.sHtML

[U28] Py：类型别名
来源：http://mobile.sjlbkw.cn/Article/details/gzcpyhdjk.sHtML

UserId = int
来源：http://m.share.yfazqb.com/Article/details/gahdyprln.sHtML

[U29] Py：属性校验
来源：http://read.share.epnwcf.com/Article/details/ggniickjj.sHtML

@property 与 @x.setter 配合
来源：http://m.share.bbcook.cn/Article/details/gtuekpdmn.sHtML

[U30] Py：数据类
来源：http://read.share.yfazqb.com/Article/details/gbklypqpn.sHtML

@dataclass(slots=True)
来源：http://3g.yfazqb.com/Article/details/gwrsziiei.sHtML

[U31] Py：单测
来源：http://mobile.vehdjk.com/Article/details/gdtpttdke.sHtML

python -m pytest -q
来源：http://www.blog.tarul.cn/Article/details/gcqoquchs.sHtML

[U32] Py：代码格式化
来源：http://m.share.tarul.cn/Article/details/gycfsvdpb.sHtML

ruff format . && ruff check --fix .
来源：http://mobile.yfazqb.com/Article/details/gbsehddxd.sHtML

[U33] Py：打包发布
来源：http://mobile.vehdjk.com/Article/details/gjdvupxgi.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://www.blog.tarul.cn/Article/details/ggkckrclg.sHtML

[U34] Py：判断编码
来源：http://m.share.bbcook.cn/Article/details/ggxyiwllp.sHtML

chardet.detect(raw)
来源：http://www.m.share.vehdjk.com/Article/details/guzdjtblc.sHtML

[U35] Py：发送邮件
来源：http://www.share.yfazqb.com/Article/details/glpdldktd.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://baike.epnwcf.com/Article/details/gyqushcvu.sHtML

[U36] Py：定时任务
来源：http://baike.tarul.cn/Article/details/gjapfjkpj.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.yfazqb.com/Article/details/gjqwkruyr.sHtML

[U37] Py：读写 Excel
来源：http://baike.sjlbkw.cn/Article/details/gxwprvlaz.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://baike.bbcook.cn/Article/details/gcffgkxol.sHtML

[U38] Py：获取脚本所在目录
来源：http://m.share.epnwcf.com/Article/details/gmflwmbke.sHtML

Path(__file__).resolve().parent
来源：http://mobile.vehdjk.com/Article/details/gcnffwltd.sHtML

[U39] Py：判断是否在交互环境
来源：http://mobile.yfazqb.com/Article/details/geayogrus.sHtML

sys.stdout.isatty()
来源：http://3g.epnwcf.com/Article/details/gnmyythcq.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.epnwcf.com/Article/details/gwhjpsucz.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.yfazqb.com/Article/details/gdypvkxej.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://blog.tarul.cn/Article/details/ggdxrrlfi.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.m.share.tarul.cn/Article/details/gkynwukfu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://3g.epnwcf.com/Article/details/ghapmzxcy.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fktsv.cn/Article/details/gfvqsdnmf.sHtML

[U43] PHP：声明命名空间
来源：http://baike.tarul.cn/Article/details/gzmhibgva.sHtML

namespace App\Http;
来源：http://wap.fktsv.cn/Article/details/golteqlju.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.sjlbkw.cn/Article/details/gtvzyifpt.sHtML

declare(strict_types=1);
来源：http://m.share.yfazqb.com/Article/details/gfcwrngtg.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.bbcook.cn/Article/details/gbtdyuiar.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.vehdjk.com/Article/details/gwtxijicx.sHtML

[U46] PHP：可空类型
来源：http://read.share.bbcook.cn/Article/details/gvynjghmx.sHtML

?string $name = null
来源：http://baike.sjlbkw.cn/Article/details/gaszmeguc.sHtML

[U47] PHP：联合类型
来源：http://www.share.epnwcf.com/Article/details/gaeivrpur.sHtML

int|string $id
来源：http://blog.yfazqb.com/Article/details/guynakhha.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.vehdjk.com/Article/details/goepodjgb.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://3g.sjlbkw.cn/Article/details/gnytagbmw.sHtML

[U49] PHP：只读属性
来源：http://3g.epnwcf.com/Article/details/gvnpnitin.sHtML

public readonly string $name
来源：http://baike.tarul.cn/Article/details/gtzvnqxrb.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.vehdjk.com/Article/details/gygbrluov.sHtML

public function __construct(private int $id) {}
来源：http://blog.epnwcf.com/Article/details/guctwbadh.sHtML

[U51] PHP：数组解构
来源：http://read.share.sjlbkw.cn/Article/details/gzcpvqzwi.sHtML

[$a, $b] = $arr;
来源：http://read.share.tarul.cn/Article/details/guqzxqwgf.sHtML

[U52] PHP：箭头函数
来源：http://m.share.tarul.cn/Article/details/gbayzvptd.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.epnwcf.com/Article/details/gqueooitj.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.sjlbkw.cn/Article/details/gnkkxvpaz.sHtML

$v = $a ?? $b ?? "default";
来源：http://m.share.epnwcf.com/Article/details/gpxoqyiut.sHtML

[U54] PHP：空安全调用
来源：http://www.share.epnwcf.com/Article/details/gbkrxreoy.sHtML

$obj?->method()
来源：http://blog.vehdjk.com/Article/details/gmxlxpptc.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.epnwcf.com/Article/details/gtfjezflt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.vehdjk.com/Article/details/gtyywuhim.sHtML

[U56] PHP：命名参数
来源：http://3g.tarul.cn/Article/details/guprgnxqh.sHtML

f(a: 1, b: 2)
来源：http://www.share.sjlbkw.cn/Article/details/gsyfxolbp.sHtML

[U57] PHP：字符串插值
来源：http://baike.yfazqb.com/Article/details/gbybmqwsm.sHtML

"值: {$a}"
来源：http://baike.fktsv.cn/Article/details/ggqfworno.sHtML

[U58] PHP：数组三件套
来源：http://m.share.epnwcf.com/Article/details/gxduqkxmh.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.sjlbkw.cn/Article/details/gikgysxhm.sHtML

[U59] PHP：自定义排序
来源：http://read.share.epnwcf.com/Article/details/glednscxj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.epnwcf.com/Article/details/gvcwisncn.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.epnwcf.com/Article/details/ghnssbrcd.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.tarul.cn/Article/details/gwypvtjql.sHtML

[U61] PHP：正则
来源：http://wap.yfazqb.com/Article/details/gxlstpnwp.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.epnwcf.com/Article/details/gxscjvbxi.sHtML

[U62] PHP：日期对象
来源：http://baike.epnwcf.com/Article/details/gxxwhgnod.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.sjlbkw.cn/Article/details/gwgatfccg.sHtML

[U63] PHP：文件读写
来源：http://3g.tarul.cn/Article/details/gytdzealv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.bbcook.cn/Article/details/gqwnlnbvn.sHtML

[U64] PHP：目录遍历
来源：http://www.share.bbcook.cn/Article/details/giuzazeyn.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.bbcook.cn/Article/details/gyxxwgfxq.sHtML

[U65] PHP：会话
来源：http://blog.yfazqb.com/Article/details/ggfkumzdl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.tarul.cn/Article/details/glvdumwlg.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.vehdjk.com/Article/details/gldmucmxa.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fktsv.cn/Article/details/gvhiyyydd.sHtML

[U67] PHP：处理文件上传
来源：http://baike.bbcook.cn/Article/details/gopdlrymo.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.bbcook.cn/Article/details/ggescvwlp.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.bbcook.cn/Article/details/gchezfmij.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.sjlbkw.cn/Article/details/gufzydosc.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.fktsv.cn/Article/details/giqzfsgra.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fktsv.cn/Article/details/gessobxmx.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.sjlbkw.cn/Article/details/gsbgssplk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.tarul.cn/Article/details/goefzpwyx.sHtML

[U71] PHP：抛出异常
来源：http://read.share.yfazqb.com/Article/details/gjpcmccnf.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fktsv.cn/Article/details/gzatkkhib.sHtML

[U72] PHP：写错误日志
来源：http://3g.bbcook.cn/Article/details/gouwqdvgl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.vehdjk.com/Article/details/ggzofbepj.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.yfazqb.com/Article/details/gabaraimn.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fktsv.cn/Article/details/gdvifixqo.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.bbcook.cn/Article/details/gbdwuzbhf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.epnwcf.com/Article/details/gndjvmlyl.sHtML

[U75] PHP：依赖注入
来源：http://www.share.vehdjk.com/Article/details/gxynllkmy.sHtML

composer require psr/container
来源：http://read.share.yfazqb.com/Article/details/gpfhtpstv.sHtML

[U76] PHP：简单路由
来源：http://www.blog.tarul.cn/Article/details/ggusfqbqy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.yfazqb.com/Article/details/gpxkoqvwh.sHtML

[U77] PHP：模板渲染
来源：http://m.share.fktsv.cn/Article/details/ggggdgksa.sHtML

composer require twig/twig
来源：http://3g.fktsv.cn/Article/details/gwczunwhj.sHtML

[U78] PHP：单元测试
来源：http://www.blog.tarul.cn/Article/details/gxutlegqu.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.yfazqb.com/Article/details/gaomqwegw.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.vehdjk.com/Article/details/gzgarqnfm.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.vehdjk.com/Article/details/gpjinqdhk.sHtML

[U80] PHP：代码规范修复
来源：http://baike.bbcook.cn/Article/details/gdapdxfrl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fktsv.cn/Article/details/gionyqlhd.sHtML

[U81] JS：初始化项目
来源：http://wap.fktsv.cn/Article/details/gbcilcvvn.sHtML

npm init -y;  npm i express
来源：http://baike.yfazqb.com/Article/details/gcqyvexdf.sHtML

[U82] JS：package.json 脚本
来源：http://3g.yfazqb.com/Article/details/gvoygjvou.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.epnwcf.com/Article/details/gxqxkkxop.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.epnwcf.com/Article/details/giezoerux.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.yfazqb.com/Article/details/gquhsftgq.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.epnwcf.com/Article/details/gwdxnzpuj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.epnwcf.com/Article/details/gbnyzvktu.sHtML

[U85] JS：可选链
来源：http://www.m.share.epnwcf.com/Article/details/grmjzrpss.sHtML

a?.b?.c
来源：http://www.share.bbcook.cn/Article/details/grunasvkz.sHtML

[U86] JS：空值合并
来源：http://blog.epnwcf.com/Article/details/gogkukkfw.sHtML

a ?? b
来源：http://3g.bbcook.cn/Article/details/gheisaffu.sHtML

[U87] JS：解构默认值
来源：http://blog.yfazqb.com/Article/details/giqocnjlf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.tarul.cn/Article/details/gcazahdio.sHtML

[U88] JS：对象展开合并
来源：http://www.share.epnwcf.com/Article/details/gpfqqntwq.sHtML

{ ...a, ...b }
来源：http://www.blog.tarul.cn/Article/details/gokfbhico.sHtML

[U89] JS：数组去重
来源：http://baike.vehdjk.com/Article/details/gwcapxehn.sHtML

[...new Set(arr)]
来源：http://wap.fktsv.cn/Article/details/guiakekgt.sHtML

[U90] JS：数字数组排序
来源：http://m.share.tarul.cn/Article/details/gkmfhgmwz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/gkyperayl.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.yfazqb.com/Article/details/gmdecbdlo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.sjlbkw.cn/Article/details/gdfbhnriw.sHtML

[U92] JS：深拷贝
来源：http://m.share.epnwcf.com/Article/details/gcxbpbgyq.sHtML

structuredClone(obj)
来源：http://read.share.yfazqb.com/Article/details/gnfhhboyr.sHtML

[U93] JS：模板字符串
来源：http://m.share.tarul.cn/Article/details/gijscvpdm.sHtML

`共 ${n} 条`
来源：http://wap.tarul.cn/Article/details/grhyjepjb.sHtML

[U94] JS：箭头函数
来源：http://3g.tarul.cn/Article/details/gvmnuleuu.sHtML

const double = x => x * 2;
来源：http://www.blog.tarul.cn/Article/details/gmqyqcfcy.sHtML

[U95] JS：Promise 包装
来源：http://3g.bbcook.cn/Article/details/gmxavajit.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.sjlbkw.cn/Article/details/glltywnci.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.sjlbkw.cn/Article/details/gtifhyivy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.bbcook.cn/Article/details/gwexbsgof.sHtML

[U97] JS：并发请求
来源：http://m.share.fktsv.cn/Article/details/guiitzzjh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/gkgddvzas.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.bbcook.cn/Article/details/gmijloegr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.bbcook.cn/Article/details/gbwjyagzy.sHtML

[U99] JS：事件监听
来源：http://www.m.share.vehdjk.com/Article/details/gkbeltvsi.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.tarul.cn/Article/details/gfjcrbovv.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.bbcook.cn/Article/details/gwouwqbmz.sHtML

document.querySelector(".item")
来源：http://read.share.sjlbkw.cn/Article/details/gokonnyoo.sHtML

[U101] JS：classList 操作
来源：http://wap.tarul.cn/Article/details/gdtyfrnhe.sHtML

el.classList.toggle("active")
来源：http://3g.sjlbkw.cn/Article/details/gqjsrbvju.sHtML

[U102] JS：本地存储
来源：http://m.share.vehdjk.com/Article/details/gwfxfdsfw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.tarul.cn/Article/details/grhrabnwh.sHtML

[U103] JS：定时器
来源：http://www.blog.sjlbkw.cn/Article/details/gctqdsdhy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.vehdjk.com/Article/details/ggnjomqlj.sHtML

[U104] JS：防抖
来源：http://blog.fktsv.cn/Article/details/giotaerpp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.epnwcf.com/Article/details/gmujnwiju.sHtML

[U105] JS：节流
来源：http://read.share.vehdjk.com/Article/details/gurlqzaom.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gvlwuxgvw.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/gewcddzkq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.tarul.cn/Article/details/gpjtrukre.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fktsv.cn/Article/details/gadokamzx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.tarul.cn/Article/details/gyhfagocw.sHtML

[U108] JS：随机整数
来源：http://wap.epnwcf.com/Article/details/gkvdcdusx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.vehdjk.com/Article/details/grahyuwby.sHtML

[U109] JS：数组分组
来源：http://mobile.sjlbkw.cn/Article/details/gknnzmjyk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fktsv.cn/Article/details/gfxcpawhc.sHtML

[U110] JS：数组分块
来源：http://blog.vehdjk.com/Article/details/gkohjkjul.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.vehdjk.com/Article/details/gighzgeii.sHtML

[U111] JS：对象转 Map
来源：http://3g.fktsv.cn/Article/details/guuejqzbb.sHtML

new Map(Object.entries(obj))
来源：http://wap.yfazqb.com/Article/details/gbdoitczl.sHtML

[U112] JS：字符串补位
来源：http://blog.epnwcf.com/Article/details/ghhgemykh.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.vehdjk.com/Article/details/gumnkkzhu.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.epnwcf.com/Article/details/gzbepapds.sHtML

s.replaceAll("a", "b")
来源：http://wap.vehdjk.com/Article/details/gfeiyiwal.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.bbcook.cn/Article/details/gmtpqvpxm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fktsv.cn/Article/details/gysrhbxly.sHtML

[U115] JS：生成 UUID
来源：http://3g.fktsv.cn/Article/details/gzurmwusi.sHtML

crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/gqtqiizrm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fktsv.cn/Article/details/gjqtvgnkf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.bbcook.cn/Article/details/gfjrgclgs.sHtML

[U117] JS：单元测试
来源：http://m.share.fktsv.cn/Article/details/ghzbvijth.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.bbcook.cn/Article/details/gkukhtjds.sHtML

[U118] JS：开发服务器
来源：http://www.blog.vehdjk.com/Article/details/gsltbpzph.sHtML

npm i -D vite;  npx vite
来源：http://m.share.epnwcf.com/Article/details/gnmpmumtg.sHtML

[U119] JS：生产构建
来源：http://3g.sjlbkw.cn/Article/details/gwmbidywd.sHtML

npx vite build
来源：http://baike.tarul.cn/Article/details/gpssxzwci.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.vehdjk.com/Article/details/gkuvavinb.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fktsv.cn/Article/details/gvvrmogdr.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gfcibvfpq.sHtML

统计汇总
来源：http://mobile.sjlbkw.cn/Article/details/gbcaxwqcp.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gsmpmflrh.sHtML

按语言统计（条）：
来源：http://www.blog.sjlbkw.cn/Article/details/ghiblcyxn.sHtML

Python ......... 252
来源：http://blog.epnwcf.com/Article/details/glabsrtnz.sHtML

PHP ............ 252
来源：http://3g.tarul.cn/Article/details/gdocshyxp.sHtML

JavaScript ..... 252
来源：http://m.share.epnwcf.com/Article/details/geewbemqh.sHtML

TypeScript ..... 212
来源：http://wap.tarul.cn/Article/details/ghhmrnqsz.sHtML

Java ........... 212
来源：http://www.m.share.yfazqb.com/Article/details/glyhaiwzo.sHtML

Go ............. 212
来源：http://blog.bbcook.cn/Article/details/gtedsyazb.sHtML

Ruby ........... 212
来源：http://m.share.bbcook.cn/Article/details/gxrdixcgg.sHtML

C# ............. 212
来源：http://wap.tarul.cn/Article/details/gocatsqwq.sHtML

C .............. 30
来源：http://m.share.fktsv.cn/Article/details/ghozwqzkl.sHtML

C++ ............ 30
来源：http://www.share.bbcook.cn/Article/details/gyfmmlvly.sHtML

SQL ............ 90
来源：http://3g.fktsv.cn/Article/details/gzafrvisl.sHtML

Bash ........... 80
来源：http://read.share.bbcook.cn/Article/details/gtmmhsubp.sHtML

Kotlin ......... 15
来源：http://www.m.share.tarul.cn/Article/details/gksksjvvd.sHtML

Swift .......... 15
来源：http://mobile.sjlbkw.cn/Article/details/gvzinceti.sHtML

Lua ............ 10
来源：http://blog.sjlbkw.cn/Article/details/gkuuejoal.sHtML

Perl ........... 10
来源：http://mobile.bbcook.cn/Article/details/gqwlrjvbe.sHtML

Scala .......... 10
来源：http://baike.fktsv.cn/Article/details/gkjelklov.sHtML

------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gryvefivu.sHtML

合计 ........... 2106 条
来源：http://blog.fktsv.cn/Article/details/gjlybmzjm.sHtML

按章节统计：
来源：http://mobile.yfazqb.com/Article/details/grqbvdouh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fktsv.cn/Article/details/gcvytrrhx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.sjlbkw.cn/Article/details/gpcsobexw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.epnwcf.com/Article/details/gkjosqqlq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fktsv.cn/Article/details/gustczsuv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.bbcook.cn/Article/details/gmtjofkyh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.yfazqb.com/Article/details/gbgaidbmb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.bbcook.cn/Article/details/gddervktt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.epnwcf.com/Article/details/gbdbuxvve.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fktsv.cn/Article/details/ghvbajois.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.tarul.cn/Article/details/gyuxhmtxz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.vehdjk.com/Article/details/galevdsnj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.bbcook.cn/Article/details/gmppgvsss.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.epnwcf.com/Article/details/gxvtzdrju.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.sjlbkw.cn/Article/details/grjonkahz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.yfazqb.com/Article/details/gesjxwvqn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/gnfohpjqb.sHtML

Q SQL 专题                              90
来源：http://wap.yfazqb.com/Article/details/grxjvmrim.sHtML

R Bash 专题                             80
来源：http://www.m.share.sjlbkw.cn/Article/details/gjktrsses.sHtML

S C / C++ 专题                          60
来源：http://read.share.tarul.cn/Article/details/gjotousoa.sHtML

T 其他语言补充                          60
来源：http://www.m.share.vehdjk.com/Article/details/gjbhjcell.sHtML

U 高频实用片段                         120
来源：http://3g.tarul.cn/Article/details/glqblljya.sHtML

------------------------------------
来源：http://blog.sjlbkw.cn/Article/details/glrbnflhw.sHtML

合计                                  2106 条
来源：http://blog.epnwcf.com/Article/details/giqojpdyu.sHtML

--------------------------------------------------------------------------------
来源：http://baike.epnwcf.com/Article/details/gpwczwbqo.sHtML

使用提醒
来源：http://blog.epnwcf.com/Article/details/gpmjxdwjn.sHtML

--------------------------------------------------------------------------------
来源：http://blog.vehdjk.com/Article/details/gxvjrkziv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.sjlbkw.cn/Article/details/gowyomtnx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fktsv.cn/Article/details/gwyeitwab.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.bbcook.cn/Article/details/gnrfohhsq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fktsv.cn/Article/details/gitmykfzx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.epnwcf.com/Article/details/gnvdgnxjq.sHtML

—— 文件结束 ——
来源：http://www.share.tarul.cn/Article/details/gzckyfsuz.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gotwkqdpl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.tarul.cn/Article/details/gxmalyley.sHtML

Common Programming Examples Cheat Book
来源：http://wap.yfazqb.com/Article/details/gcpdtvgwp.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gidpkwkfc.sHtML


<!-- 参考信息 -->