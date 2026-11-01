代发 wailian999

[U03] Py：加载 .env 配置
来源：http://mobile.vehdjk.com/Article/details/grppmeocp.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.tarul.cn/Article/details/gnlrlotgq.sHtML

[U04] Py：变量调试打印
来源：http://read.share.bbcook.cn/Article/details/gxawuysml.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.yfazqb.com/Article/details/ggwevvipm.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.bbcook.cn/Article/details/gghoprvze.sHtML

list(dict.fromkeys(arr))
来源：http://mobile.yfazqb.com/Article/details/glgaooawd.sHtML

[U06] Py：合并两个字典
来源：http://baike.yfazqb.com/Article/details/grixieaec.sHtML

{**a, **b}
来源：http://blog.vehdjk.com/Article/details/gxkzrdbzj.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fktsv.cn/Article/details/gnjluikkk.sHtML

{v: k for k, v in d.items()}
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkswujww.sHtML

[U08] Py：展平二维列表
来源：http://wap.bbcook.cn/Article/details/gtonazcnu.sHtML

[y for x in nested for y in x]
来源：http://read.share.tarul.cn/Article/details/gmgqqbcrw.sHtML

[U09] Py：字典取最大值的键
来源：http://www.blog.tarul.cn/Article/details/gcyzfvhrs.sHtML

max(d, key=d.get)
来源：http://wap.fktsv.cn/Article/details/gdtztqbwn.sHtML

[U10] Py：按值排序字典
来源：http://read.share.epnwcf.com/Article/details/gyjkzmmhq.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.blog.yfazqb.com/Article/details/gykmfgwqs.sHtML

[U11] Py：生成器表达式
来源：http://www.m.share.bbcook.cn/Article/details/gsfeesffb.sHtML

(x * 2 for x in arr)
来源：http://m.share.fktsv.cn/Article/details/gafkeqwsl.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://read.share.fktsv.cn/Article/details/gjrdnahwf.sHtML

Counter(arr).most_common(3)
来源：http://m.share.epnwcf.com/Article/details/gqcsgojyy.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fktsv.cn/Article/details/glohlwxmv.sHtML

deque(maxlen=10)
来源：http://www.share.tarul.cn/Article/details/gxykqsqtp.sHtML

[U14] Py：分组收集到列表
来源：http://3g.sjlbkw.cn/Article/details/gouuebxie.sHtML

defaultdict(list)
来源：http://blog.sjlbkw.cn/Article/details/gpxdvoknk.sHtML

[U15] Py：高精度计时
来源：http://blog.epnwcf.com/Article/details/gafzdedvn.sHtML

t = time.perf_counter()
来源：http://m.share.vehdjk.com/Article/details/giqdavljq.sHtML

[U16] Py：命令行参数解析
来源：http://wap.sjlbkw.cn/Article/details/gyydqvdee.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baike.vehdjk.com/Article/details/gtmifgfrd.sHtML

[U17] Py：初始化日志
来源：http://baike.fktsv.cn/Article/details/ghopjaoys.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://www.blog.sjlbkw.cn/Article/details/gxjzvmbwy.sHtML

[U18] Py：预编译正则
来源：http://wap.bbcook.cn/Article/details/gatsxyddj.sHtML

pat = re.compile(r"\d+")
来源：http://baike.tarul.cn/Article/details/gyoigbusf.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.tarul.cn/Article/details/gtxrzhzuv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://m.share.bbcook.cn/Article/details/gptkvlrxf.sHtML

[U20] Py：缓存函数结果
来源：http://wap.epnwcf.com/Article/details/gfdokaerz.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.share.bbcook.cn/Article/details/gljjzumgy.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.vehdjk.com/Article/details/gybiezdcd.sHtML

@contextlib.contextmanager
来源：http://baike.fktsv.cn/Article/details/gjcrfujll.sHtML

[U22] Py：矩阵转置
来源：http://www.m.share.vehdjk.com/Article/details/gtpicfucn.sHtML

list(zip(*m))
来源：http://www.share.tarul.cn/Article/details/gwfjybqol.sHtML

[U23] Py：分块读取大文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gaaxgropj.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.blog.vehdjk.com/Article/details/gdqsfhbrk.sHtML

[U24] Py：路径操作
来源：http://wap.yfazqb.com/Article/details/gpgmtuzkf.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.share.tarul.cn/Article/details/gvznzvujx.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.vehdjk.com/Article/details/gjlcocven.sHtML

csv.DictReader(f)
来源：http://www.m.share.tarul.cn/Article/details/gooxoyrzy.sHtML

[U26] Py：并发下载
来源：http://blog.bbcook.cn/Article/details/gwxpthquh.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wap.epnwcf.com/Article/details/gueoaohbn.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.vehdjk.com/Article/details/gpxjlbnah.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.epnwcf.com/Article/details/glxlvquhi.sHtML

[U28] Py：类型别名
来源：http://www.blog.yfazqb.com/Article/details/gnfgtlhid.sHtML

UserId = int
来源：http://mobile.bbcook.cn/Article/details/gbsxiuvjm.sHtML

[U29] Py：属性校验
来源：http://read.share.sjlbkw.cn/Article/details/gogrkvpoo.sHtML

@property 与 @x.setter 配合
来源：http://mobile.yfazqb.com/Article/details/grsshjxoe.sHtML

[U30] Py：数据类
来源：http://wap.fktsv.cn/Article/details/ghnlttffw.sHtML

@dataclass(slots=True)
来源：http://www.share.bbcook.cn/Article/details/gcvkpuwlm.sHtML

[U31] Py：单测
来源：http://www.m.share.yfazqb.com/Article/details/gwontnnuj.sHtML

python -m pytest -q
来源：http://m.share.sjlbkw.cn/Article/details/gszcsrihj.sHtML

[U32] Py：代码格式化
来源：http://read.share.fktsv.cn/Article/details/godvlmmcq.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.yfazqb.com/Article/details/gbgsbrjae.sHtML

[U33] Py：打包发布
来源：http://wap.vehdjk.com/Article/details/gztaxsswk.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://3g.epnwcf.com/Article/details/glmwgxcth.sHtML

[U34] Py：判断编码
来源：http://mobile.yfazqb.com/Article/details/guagigqqu.sHtML

chardet.detect(raw)
来源：http://mobile.bbcook.cn/Article/details/gfhgarxwn.sHtML

[U35] Py：发送邮件
来源：http://m.share.vehdjk.com/Article/details/gxnitpfxp.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mobile.vehdjk.com/Article/details/gifylaqqd.sHtML

[U36] Py：定时任务
来源：http://blog.fktsv.cn/Article/details/giceznefj.sHtML

schedule.every(10).minutes.do(job)
来源：http://read.share.bbcook.cn/Article/details/gzuiymnjm.sHtML

[U37] Py：读写 Excel
来源：http://wap.vehdjk.com/Article/details/grwktgzzg.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://read.share.vehdjk.com/Article/details/gwgjgrpqp.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.epnwcf.com/Article/details/gataoegfo.sHtML

Path(__file__).resolve().parent
来源：http://3g.bbcook.cn/Article/details/gjrfzqnab.sHtML

[U39] Py：判断是否在交互环境
来源：http://wap.fktsv.cn/Article/details/gjcaakcxu.sHtML

sys.stdout.isatty()
来源：http://wap.sjlbkw.cn/Article/details/gijfgmtsx.sHtML

[U40] Py：打印到标准错误
来源：http://wap.epnwcf.com/Article/details/ghoffghkh.sHtML

print("err", file=sys.stderr)
来源：http://www.blog.vehdjk.com/Article/details/gxddjxjwy.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://m.share.sjlbkw.cn/Article/details/gfhznefcx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.sjlbkw.cn/Article/details/gumttglbh.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.bbcook.cn/Article/details/ggczplvzt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.yfazqb.com/Article/details/gnixnbnmz.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.epnwcf.com/Article/details/gnksdyllz.sHtML

namespace App\Http;
来源：http://baike.sjlbkw.cn/Article/details/guqkgpjob.sHtML

[U44] PHP：开启严格类型
来源：http://wap.yfazqb.com/Article/details/gupmkbdrn.sHtML

declare(strict_types=1);
来源：http://wap.yfazqb.com/Article/details/gngyhwimj.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.sjlbkw.cn/Article/details/gznkagunr.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.vehdjk.com/Article/details/gqyldjemt.sHtML

[U46] PHP：可空类型
来源：http://3g.yfazqb.com/Article/details/gwiahkbvw.sHtML

?string $name = null
来源：http://baike.yfazqb.com/Article/details/gfupqzzly.sHtML

[U47] PHP：联合类型
来源：http://wap.sjlbkw.cn/Article/details/gbyfmlzur.sHtML

int|string $id
来源：http://www.share.fktsv.cn/Article/details/gwvrsetlq.sHtML

[U48] PHP：纯枚举
来源：http://blog.epnwcf.com/Article/details/grrkniqyx.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.yfazqb.com/Article/details/gxzqkcypk.sHtML

[U49] PHP：只读属性
来源：http://mobile.yfazqb.com/Article/details/gohhowbrr.sHtML

public readonly string $name
来源：http://3g.fktsv.cn/Article/details/ghdowikid.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.epnwcf.com/Article/details/gbgrdjzfa.sHtML

public function __construct(private int $id) {}
来源：http://mobile.fktsv.cn/Article/details/gdboqhueu.sHtML

[U51] PHP：数组解构
来源：http://3g.tarul.cn/Article/details/gsrnfotrw.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.tarul.cn/Article/details/gvcmklfuk.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.bbcook.cn/Article/details/gadoqmric.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fktsv.cn/Article/details/gueiyyeua.sHtML

[U53] PHP：空合并运算符
来源：http://blog.epnwcf.com/Article/details/glnxgwbld.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.tarul.cn/Article/details/gjnmnglge.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fktsv.cn/Article/details/ggxqbrgkq.sHtML

$obj?->method()
来源：http://m.share.fktsv.cn/Article/details/gzbwtbgtt.sHtML

[U55] PHP：match 表达式
来源：http://m.share.fktsv.cn/Article/details/gvezgmfjn.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fktsv.cn/Article/details/gjrffgdcp.sHtML

[U56] PHP：命名参数
来源：http://mobile.fktsv.cn/Article/details/gwfshwbui.sHtML

f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gjrghbwdd.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fktsv.cn/Article/details/geuyjhalc.sHtML

"值: {$a}"
来源：http://mobile.vehdjk.com/Article/details/gdahurgvp.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fktsv.cn/Article/details/gqpmishiv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.epnwcf.com/Article/details/gsvclkavu.sHtML

[U59] PHP：自定义排序
来源：http://wap.bbcook.cn/Article/details/gksqsaexq.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.vehdjk.com/Article/details/gkffxfefn.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.epnwcf.com/Article/details/gijpovmvq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.yfazqb.com/Article/details/ghxwevhei.sHtML

[U61] PHP：正则
来源：http://baike.tarul.cn/Article/details/gmdhglzmq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fktsv.cn/Article/details/gymlgvitg.sHtML

[U62] PHP：日期对象
来源：http://www.blog.tarul.cn/Article/details/gloxkkszh.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.tarul.cn/Article/details/gbhqtodph.sHtML

[U63] PHP：文件读写
来源：http://wap.sjlbkw.cn/Article/details/galumrudj.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.sjlbkw.cn/Article/details/gblrffybw.sHtML

[U64] PHP：目录遍历
来源：http://read.share.bbcook.cn/Article/details/gjksxmres.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fktsv.cn/Article/details/gipeutpoh.sHtML

[U65] PHP：会话
来源：http://read.share.bbcook.cn/Article/details/gfbmlbpxr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.epnwcf.com/Article/details/gigbhstda.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.fktsv.cn/Article/details/gajfldovu.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.bbcook.cn/Article/details/gxbxvbvxo.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.yfazqb.com/Article/details/gtzpdgvsu.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fktsv.cn/Article/details/gyjeyzpxd.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.sjlbkw.cn/Article/details/govkebydy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.vehdjk.com/Article/details/grjiyfhsu.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.yfazqb.com/Article/details/gleqiygxp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.vehdjk.com/Article/details/gpvsowuhr.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.sjlbkw.cn/Article/details/gdjgiuwdx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.bbcook.cn/Article/details/gdqomlwzn.sHtML

[U71] PHP：抛出异常
来源：http://blog.epnwcf.com/Article/details/gfhicejib.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.sjlbkw.cn/Article/details/gwpwzaxvx.sHtML

[U72] PHP：写错误日志
来源：http://baike.vehdjk.com/Article/details/gxmljpuwb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.tarul.cn/Article/details/gzreyqzqz.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.epnwcf.com/Article/details/gvhodjvmt.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.bbcook.cn/Article/details/gmtwzdwpf.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.sjlbkw.cn/Article/details/goqgwujam.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.yfazqb.com/Article/details/gqxkotlfa.sHtML

[U75] PHP：依赖注入
来源：http://m.share.yfazqb.com/Article/details/ggfwgixep.sHtML

composer require psr/container
来源：http://m.share.sjlbkw.cn/Article/details/gjwxcsdzj.sHtML

[U76] PHP：简单路由
来源：http://mobile.bbcook.cn/Article/details/grbvulyvd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.yfazqb.com/Article/details/gcnsvlwpn.sHtML

[U77] PHP：模板渲染
来源：http://read.share.tarul.cn/Article/details/gaunshyek.sHtML

composer require twig/twig
来源：http://mobile.bbcook.cn/Article/details/gwxjcmbnh.sHtML

[U78] PHP：单元测试
来源：http://read.share.sjlbkw.cn/Article/details/gxeozlmju.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.bbcook.cn/Article/details/ggoxlzpdn.sHtML

[U79] PHP：静态分析
来源：http://www.share.bbcook.cn/Article/details/gyxqzlctx.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.tarul.cn/Article/details/gvkgojynl.sHtML

[U80] PHP：代码规范修复
来源：http://blog.epnwcf.com/Article/details/gttkhbbjh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.sjlbkw.cn/Article/details/gnowejrjy.sHtML

[U81] JS：初始化项目
来源：http://blog.yfazqb.com/Article/details/guuevbvek.sHtML

npm init -y;  npm i express
来源：http://blog.fktsv.cn/Article/details/glojvclio.sHtML

[U82] JS：package.json 脚本
来源：http://blog.bbcook.cn/Article/details/gngwvuazo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.sjlbkw.cn/Article/details/gtgeqpmaj.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.bbcook.cn/Article/details/gqtowzyqg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.yfazqb.com/Article/details/gbtczeayi.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.epnwcf.com/Article/details/gaycngyqd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.epnwcf.com/Article/details/gtxjhqumy.sHtML

[U85] JS：可选链
来源：http://www.blog.epnwcf.com/Article/details/gfusiblim.sHtML

a?.b?.c
来源：http://www.blog.tarul.cn/Article/details/gjieihnvg.sHtML

[U86] JS：空值合并
来源：http://mobile.vehdjk.com/Article/details/gtftjqaxk.sHtML

a ?? b
来源：http://baike.yfazqb.com/Article/details/giupednqf.sHtML

[U87] JS：解构默认值
来源：http://www.blog.fktsv.cn/Article/details/ghorhvjdj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.epnwcf.com/Article/details/garvsxyrx.sHtML

[U88] JS：对象展开合并
来源：http://www.share.bbcook.cn/Article/details/gxvdsvnkk.sHtML

{ ...a, ...b }
来源：http://www.m.share.tarul.cn/Article/details/gfsbbncxr.sHtML

[U89] JS：数组去重
来源：http://3g.epnwcf.com/Article/details/gpvhvnpvz.sHtML

[...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/gfxfpjvio.sHtML

[U90] JS：数字数组排序
来源：http://www.share.fktsv.cn/Article/details/gajkaebgu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.sjlbkw.cn/Article/details/gddvojgin.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fktsv.cn/Article/details/gcjhgyngc.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.tarul.cn/Article/details/gzwfnqgck.sHtML

[U92] JS：深拷贝
来源：http://blog.tarul.cn/Article/details/grvkvdlcu.sHtML

structuredClone(obj)
来源：http://www.blog.epnwcf.com/Article/details/gwzyvrznv.sHtML

[U93] JS：模板字符串
来源：http://www.share.tarul.cn/Article/details/gceuxabky.sHtML

`共 ${n} 条`
来源：http://www.blog.fktsv.cn/Article/details/gxpyreasz.sHtML

[U94] JS：箭头函数
来源：http://m.share.fktsv.cn/Article/details/gkqjavlcc.sHtML

const double = x => x * 2;
来源：http://read.share.tarul.cn/Article/details/gklcjexue.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.tarul.cn/Article/details/gthxjspjl.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.bbcook.cn/Article/details/gqyiqzcrx.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.vehdjk.com/Article/details/gvuigmvbc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.tarul.cn/Article/details/gkihowmus.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fktsv.cn/Article/details/gnlbnsvfl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.tarul.cn/Article/details/gdrhoxvmd.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.epnwcf.com/Article/details/gtpvgxjhe.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.tarul.cn/Article/details/gdrycckea.sHtML

[U99] JS：事件监听
来源：http://m.share.bbcook.cn/Article/details/gfskdzjxd.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.epnwcf.com/Article/details/gngmccapi.sHtML

[U100] JS：DOM 查询
来源：http://blog.fktsv.cn/Article/details/gorkoznys.sHtML

document.querySelector(".item")
来源：http://m.share.sjlbkw.cn/Article/details/gsnpcduzu.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.sjlbkw.cn/Article/details/gqaahucoq.sHtML

el.classList.toggle("active")
来源：http://baike.epnwcf.com/Article/details/gzzllvbov.sHtML

[U102] JS：本地存储
来源：http://www.share.vehdjk.com/Article/details/groyxotng.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.yfazqb.com/Article/details/goiqasxjr.sHtML

[U103] JS：定时器
来源：http://www.blog.sjlbkw.cn/Article/details/gdxufaijb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.sjlbkw.cn/Article/details/gqsitqgsm.sHtML

[U104] JS：防抖
来源：http://blog.vehdjk.com/Article/details/gjnhdpsfa.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.yfazqb.com/Article/details/gopuxopdv.sHtML

[U105] JS：节流
来源：http://www.blog.fktsv.cn/Article/details/glwzunlun.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.bbcook.cn/Article/details/gezyjtwep.sHtML

[U106] JS：日期格式化
来源：http://www.share.epnwcf.com/Article/details/gztzklcbu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.vehdjk.com/Article/details/gwdvavgtv.sHtML

[U107] JS：数字千分位
来源：http://m.share.fktsv.cn/Article/details/gyfvhriyu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.bbcook.cn/Article/details/gvtlwxove.sHtML

[U108] JS：随机整数
来源：http://read.share.tarul.cn/Article/details/grnyzfzgx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.vehdjk.com/Article/details/guzwhxmvi.sHtML

[U109] JS：数组分组
来源：http://www.share.epnwcf.com/Article/details/gfmhgqefj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.vehdjk.com/Article/details/gyfqnvxoa.sHtML

[U110] JS：数组分块
来源：http://www.share.tarul.cn/Article/details/groxilmjj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fktsv.cn/Article/details/glludnhqe.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.yfazqb.com/Article/details/gdbgvxkpe.sHtML

new Map(Object.entries(obj))
来源：http://3g.bbcook.cn/Article/details/ghcvkevdz.sHtML

[U112] JS：字符串补位
来源：http://mobile.epnwcf.com/Article/details/gsffzqfkv.sHtML

"7".padStart(3, "0")
来源：http://www.share.fktsv.cn/Article/details/gcslmjetq.sHtML

[U113] JS：正则替换全部
来源：http://read.share.bbcook.cn/Article/details/gpefdxefd.sHtML

s.replaceAll("a", "b")
来源：http://www.share.epnwcf.com/Article/details/gcwukuzrv.sHtML

[U114] JS：JSON 深比较
来源：http://baike.epnwcf.com/Article/details/gnjmifvjn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.yfazqb.com/Article/details/gjevuybog.sHtML

[U115] JS：生成 UUID
来源：http://m.share.yfazqb.com/Article/details/gqtyqjgeu.sHtML

crypto.randomUUID()
来源：http://www.blog.vehdjk.com/Article/details/gfqeurfbb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fktsv.cn/Article/details/gmazjjpvw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.vehdjk.com/Article/details/gneqtcuky.sHtML

[U117] JS：单元测试
来源：http://m.share.sjlbkw.cn/Article/details/gkqiuhewi.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fktsv.cn/Article/details/grfexvzow.sHtML

[U118] JS：开发服务器
来源：http://blog.vehdjk.com/Article/details/guqrkwekb.sHtML

npm i -D vite;  npx vite
来源：http://blog.sjlbkw.cn/Article/details/gamrdiwfg.sHtML

[U119] JS：生产构建
来源：http://m.share.sjlbkw.cn/Article/details/gakihdqrg.sHtML

npx vite build
来源：http://m.share.tarul.cn/Article/details/gxqwpxbkw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.vehdjk.com/Article/details/gkpqgbrox.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.bbcook.cn/Article/details/ggcvhksgu.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gxaksyvvr.sHtML

统计汇总
来源：http://baike.yfazqb.com/Article/details/gunptztms.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gsrmckngh.sHtML

按语言统计（条）：
来源：http://3g.fktsv.cn/Article/details/gxyzwlqor.sHtML

Python ......... 252
来源：http://www.share.sjlbkw.cn/Article/details/gepcdomjt.sHtML

PHP ............ 252
来源：http://www.m.share.tarul.cn/Article/details/gufrtqzmk.sHtML

JavaScript ..... 252
来源：http://3g.fktsv.cn/Article/details/gtpxulnwd.sHtML

TypeScript ..... 212
来源：http://mobile.yfazqb.com/Article/details/gauvenscm.sHtML

Java ........... 212
来源：http://www.m.share.sjlbkw.cn/Article/details/guovlkkts.sHtML

Go ............. 212
来源：http://m.share.epnwcf.com/Article/details/gmrtrtlcd.sHtML

Ruby ........... 212
来源：http://wap.bbcook.cn/Article/details/gogqpdbyk.sHtML

C# ............. 212
来源：http://www.share.sjlbkw.cn/Article/details/gnmoagqei.sHtML

C .............. 30
来源：http://3g.vehdjk.com/Article/details/gyyoajpva.sHtML

C++ ............ 30
来源：http://wap.vehdjk.com/Article/details/gcycopckc.sHtML

SQL ............ 90
来源：http://wap.fktsv.cn/Article/details/gnjswmtcy.sHtML

Bash ........... 80
来源：http://www.m.share.sjlbkw.cn/Article/details/gicqyclcv.sHtML

Kotlin ......... 15
来源：http://www.blog.tarul.cn/Article/details/gkukchwlp.sHtML

Swift .......... 15
来源：http://www.m.share.fktsv.cn/Article/details/gelecwaou.sHtML

Lua ............ 10
来源：http://baike.fktsv.cn/Article/details/gwpksrwxz.sHtML

Perl ........... 10
来源：http://baike.bbcook.cn/Article/details/guyxuubzp.sHtML

Scala .......... 10
来源：http://blog.fktsv.cn/Article/details/gaghiuuvz.sHtML

------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/glkyxeeck.sHtML

合计 ........... 2106 条
来源：http://baike.yfazqb.com/Article/details/gcoktjmui.sHtML

按章节统计：
来源：http://read.share.yfazqb.com/Article/details/giehhpqgh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fktsv.cn/Article/details/gahlldlnp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.bbcook.cn/Article/details/gseiszhns.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.epnwcf.com/Article/details/glksfjxqq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.bbcook.cn/Article/details/gqdtuigdw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.sjlbkw.cn/Article/details/gkptevuyh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.yfazqb.com/Article/details/gnumyitco.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.tarul.cn/Article/details/gmjcykund.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.epnwcf.com/Article/details/gambkzmqm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.vehdjk.com/Article/details/gmmtroslf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.vehdjk.com/Article/details/gjurluvxt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.tarul.cn/Article/details/gupxqbwsm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gugznqwgi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.tarul.cn/Article/details/glvnwungb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.bbcook.cn/Article/details/goifpwchy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.tarul.cn/Article/details/gsiiobnmi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.vehdjk.com/Article/details/gpyhyodva.sHtML

Q SQL 专题                              90
来源：http://www.share.tarul.cn/Article/details/gheuqcxgx.sHtML

R Bash 专题                             80
来源：http://m.share.vehdjk.com/Article/details/gwhvjjacc.sHtML

S C / C++ 专题                          60
来源：http://blog.sjlbkw.cn/Article/details/gsommedmj.sHtML

T 其他语言补充                          60
来源：http://www.m.share.tarul.cn/Article/details/gxqvukktm.sHtML

U 高频实用片段                         120
来源：http://mobile.epnwcf.com/Article/details/gwjxefmrd.sHtML

------------------------------------
来源：http://read.share.tarul.cn/Article/details/gfjqkdxbr.sHtML

合计                                  2106 条
来源：http://mobile.yfazqb.com/Article/details/geuwmhoyt.sHtML

--------------------------------------------------------------------------------
来源：http://wap.bbcook.cn/Article/details/gcnpyypok.sHtML

使用提醒
来源：http://blog.vehdjk.com/Article/details/gayykxcht.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.vehdjk.com/Article/details/grtjhkzki.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.vehdjk.com/Article/details/gxaidpfqs.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.vehdjk.com/Article/details/gdwdonsob.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.yfazqb.com/Article/details/gnorlgrmf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.tarul.cn/Article/details/gbptjkhea.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fktsv.cn/Article/details/gidsoshxq.sHtML

—— 文件结束 ——
来源：http://www.m.share.yfazqb.com/Article/details/gtctsdsgy.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gxanxsudb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.yfazqb.com/Article/details/gxjsspccp.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fktsv.cn/Article/details/gjqvmimxn.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gxixjzcjd.sHtML

【收录内容】
来源：http://m.share.sjlbkw.cn/Article/details/gjssliosl.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.bbcook.cn/Article/details/gfhpixeav.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fktsv.cn/Article/details/gduaoggbh.sHtML

SQL · Bash · C · C++
来源：http://read.share.yfazqb.com/Article/details/gqcxxrmiq.sHtML


<!-- 参考信息 -->