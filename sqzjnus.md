代发 wailian999

[U03] Py：加载 .env 配置
来源：http://m.share.yfazqb.com/Article/details/gowjqftsx.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.fktsv.cn/Article/details/gvmwlktvg.sHtML

[U04] Py：变量调试打印
来源：http://www.share.vehdjk.com/Article/details/gifwmyzoi.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.share.sjlbkw.cn/Article/details/gwmnczjsz.sHtML

[U05] Py：列表去重且保序
来源：http://www.m.share.epnwcf.com/Article/details/gljwfcknk.sHtML

list(dict.fromkeys(arr))
来源：http://www.m.share.yfazqb.com/Article/details/gxlgbsixh.sHtML

[U06] Py：合并两个字典
来源：http://wap.yfazqb.com/Article/details/gzmbnejnd.sHtML

{**a, **b}
来源：http://www.blog.yfazqb.com/Article/details/gyfxzqpoa.sHtML

[U07] Py：反转字典键值
来源：http://www.m.share.yfazqb.com/Article/details/gjzibnqav.sHtML

{v: k for k, v in d.items()}
来源：http://www.share.tarul.cn/Article/details/gxaqcdwbg.sHtML

[U08] Py：展平二维列表
来源：http://baike.bbcook.cn/Article/details/gxrtwyinu.sHtML

[y for x in nested for y in x]
来源：http://m.share.fktsv.cn/Article/details/gonbljqtr.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.epnwcf.com/Article/details/gsycejqxl.sHtML

max(d, key=d.get)
来源：http://www.blog.sjlbkw.cn/Article/details/gxkrdaehb.sHtML

[U10] Py：按值排序字典
来源：http://3g.tarul.cn/Article/details/gfkbohflo.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://baike.fktsv.cn/Article/details/gpccxrpyd.sHtML

[U11] Py：生成器表达式
来源：http://www.share.sjlbkw.cn/Article/details/gpjrllhrb.sHtML

(x * 2 for x in arr)
来源：http://www.blog.tarul.cn/Article/details/gqojkbeft.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://3g.epnwcf.com/Article/details/gwpdnasyd.sHtML

Counter(arr).most_common(3)
来源：http://wap.bbcook.cn/Article/details/grpccjyvs.sHtML

[U13] Py：固定长度队列
来源：http://www.blog.yfazqb.com/Article/details/gehxxoobv.sHtML

deque(maxlen=10)
来源：http://baike.yfazqb.com/Article/details/gpsagehkr.sHtML

[U14] Py：分组收集到列表
来源：http://3g.sjlbkw.cn/Article/details/ggbkoriup.sHtML

defaultdict(list)
来源：http://www.m.share.epnwcf.com/Article/details/gfgtdpwju.sHtML

[U15] Py：高精度计时
来源：http://read.share.yfazqb.com/Article/details/gadxguseh.sHtML

t = time.perf_counter()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqqpujvg.sHtML

[U16] Py：命令行参数解析
来源：http://mobile.yfazqb.com/Article/details/guocrpaxr.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://m.share.tarul.cn/Article/details/gozckutgo.sHtML

[U17] Py：初始化日志
来源：http://www.blog.epnwcf.com/Article/details/gsnahrbhx.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.vehdjk.com/Article/details/gqgyydvno.sHtML

[U18] Py：预编译正则
来源：http://www.blog.sjlbkw.cn/Article/details/geidczxzh.sHtML

pat = re.compile(r"\d+")
来源：http://baike.fktsv.cn/Article/details/grdtfnbaj.sHtML

[U19] Py：正则替换带回调
来源：http://www.blog.fktsv.cn/Article/details/gzelqytcv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.share.fktsv.cn/Article/details/gjfbixtoh.sHtML

[U20] Py：缓存函数结果
来源：http://wap.sjlbkw.cn/Article/details/gngwpmzgl.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.m.share.tarul.cn/Article/details/gvaquxvst.sHtML

[U21] Py：自定义上下文管理器
来源：http://blog.tarul.cn/Article/details/gtiscfzbt.sHtML

@contextlib.contextmanager
来源：http://www.m.share.vehdjk.com/Article/details/grnfacjbz.sHtML

[U22] Py：矩阵转置
来源：http://m.share.epnwcf.com/Article/details/gclwsllgc.sHtML

list(zip(*m))
来源：http://read.share.tarul.cn/Article/details/gkybqtpej.sHtML

[U23] Py：分块读取大文件
来源：http://3g.epnwcf.com/Article/details/gfwrbxehd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://blog.yfazqb.com/Article/details/glhhgkqaz.sHtML

[U24] Py：路径操作
来源：http://m.share.epnwcf.com/Article/details/gxvzznket.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.blog.tarul.cn/Article/details/gyckuxiyz.sHtML

[U25] Py：CSV 按字典读
来源：http://baike.epnwcf.com/Article/details/gzifgzdtg.sHtML

csv.DictReader(f)
来源：http://baike.yfazqb.com/Article/details/gkqydpukf.sHtML

[U26] Py：并发下载
来源：http://baike.fktsv.cn/Article/details/gbkbyciqt.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.epnwcf.com/Article/details/gtkhvztdr.sHtML

[U27] Py：异步 HTTP
来源：http://read.share.sjlbkw.cn/Article/details/gqlbxuqhe.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://read.share.vehdjk.com/Article/details/geluzofid.sHtML

[U28] Py：类型别名
来源：http://www.share.yfazqb.com/Article/details/graxtszti.sHtML

UserId = int
来源：http://3g.yfazqb.com/Article/details/gyivdzlwu.sHtML

[U29] Py：属性校验
来源：http://3g.epnwcf.com/Article/details/gchqulsrj.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.tarul.cn/Article/details/gxmmhqbyn.sHtML

[U30] Py：数据类
来源：http://www.blog.tarul.cn/Article/details/gwhkibvzx.sHtML

@dataclass(slots=True)
来源：http://www.m.share.epnwcf.com/Article/details/garhsbtxa.sHtML

[U31] Py：单测
来源：http://www.m.share.bbcook.cn/Article/details/gbebtrafl.sHtML

python -m pytest -q
来源：http://www.share.yfazqb.com/Article/details/gyeadymnq.sHtML

[U32] Py：代码格式化
来源：http://www.share.bbcook.cn/Article/details/ghyfyvesq.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.fktsv.cn/Article/details/gupogcarv.sHtML

[U33] Py：打包发布
来源：http://read.share.tarul.cn/Article/details/gapdacgiz.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.vehdjk.com/Article/details/gqvnkjnqn.sHtML

[U34] Py：判断编码
来源：http://m.share.sjlbkw.cn/Article/details/gqcwungfl.sHtML

chardet.detect(raw)
来源：http://m.share.fktsv.cn/Article/details/gebxnxtgh.sHtML

[U35] Py：发送邮件
来源：http://wap.bbcook.cn/Article/details/gnayfmpzn.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.epnwcf.com/Article/details/gdakkwbwy.sHtML

[U36] Py：定时任务
来源：http://read.share.vehdjk.com/Article/details/gsdfddgdt.sHtML

schedule.every(10).minutes.do(job)
来源：http://blog.epnwcf.com/Article/details/gdxrbeqfa.sHtML

[U37] Py：读写 Excel
来源：http://blog.tarul.cn/Article/details/gfuxbwatm.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.sjlbkw.cn/Article/details/ghjwwrwyi.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.share.yfazqb.com/Article/details/gnkxqlwvy.sHtML

Path(__file__).resolve().parent
来源：http://www.m.share.yfazqb.com/Article/details/glufqqawg.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.share.tarul.cn/Article/details/grwlxgjom.sHtML

sys.stdout.isatty()
来源：http://baike.vehdjk.com/Article/details/gnuunnzyb.sHtML

[U40] Py：打印到标准错误
来源：http://read.share.vehdjk.com/Article/details/gnepjyvad.sHtML

print("err", file=sys.stderr)
来源：http://wap.tarul.cn/Article/details/ggeuyimib.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.yfazqb.com/Article/details/gbponwniq.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.yfazqb.com/Article/details/gceljxbcg.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.bbcook.cn/Article/details/ggrzfabzv.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.bbcook.cn/Article/details/gwioojiqj.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.yfazqb.com/Article/details/ggbqndciu.sHtML

namespace App\Http;
来源：http://read.share.sjlbkw.cn/Article/details/goymavtat.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.sjlbkw.cn/Article/details/gsmngfgvk.sHtML

declare(strict_types=1);
来源：http://www.blog.tarul.cn/Article/details/gvtxkaipz.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.yfazqb.com/Article/details/gjgfstigu.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.sjlbkw.cn/Article/details/ggcqhiddu.sHtML

[U46] PHP：可空类型
来源：http://m.share.sjlbkw.cn/Article/details/gddwlbnah.sHtML

?string $name = null
来源：http://wap.vehdjk.com/Article/details/gnbpmkxzh.sHtML

[U47] PHP：联合类型
来源：http://www.blog.yfazqb.com/Article/details/gvwvwlfop.sHtML

int|string $id
来源：http://3g.yfazqb.com/Article/details/gdcvtpwlp.sHtML

[U48] PHP：纯枚举
来源：http://wap.tarul.cn/Article/details/gwlaerpuc.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.yfazqb.com/Article/details/gmflrxzeq.sHtML

[U49] PHP：只读属性
来源：http://baike.yfazqb.com/Article/details/gtfjeoryg.sHtML

public readonly string $name
来源：http://m.share.epnwcf.com/Article/details/ghundvzar.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.bbcook.cn/Article/details/gjsouworf.sHtML

public function __construct(private int $id) {}
来源：http://www.share.yfazqb.com/Article/details/gboeaailr.sHtML

[U51] PHP：数组解构
来源：http://mobile.sjlbkw.cn/Article/details/guhywogrb.sHtML

[$a, $b] = $arr;
来源：http://blog.bbcook.cn/Article/details/gqjsmjxhl.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.bbcook.cn/Article/details/gbqjlyndv.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.yfazqb.com/Article/details/goowqnhlh.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.epnwcf.com/Article/details/gukjxpmpf.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.vehdjk.com/Article/details/gntgirohp.sHtML

[U54] PHP：空安全调用
来源：http://blog.yfazqb.com/Article/details/guyfiebow.sHtML

$obj?->method()
来源：http://wap.fktsv.cn/Article/details/gstelmqnl.sHtML

[U55] PHP：match 表达式
来源：http://mobile.yfazqb.com/Article/details/gezdmgfyw.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.yfazqb.com/Article/details/gxormmhov.sHtML

[U56] PHP：命名参数
来源：http://blog.vehdjk.com/Article/details/gfrwmlohe.sHtML

f(a: 1, b: 2)
来源：http://read.share.yfazqb.com/Article/details/gduykkynd.sHtML

[U57] PHP：字符串插值
来源：http://blog.bbcook.cn/Article/details/gnlkcoeke.sHtML

"值: {$a}"
来源：http://baike.bbcook.cn/Article/details/gttbclloz.sHtML

[U58] PHP：数组三件套
来源：http://3g.vehdjk.com/Article/details/gajilsmew.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.yfazqb.com/Article/details/gczzueogo.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.epnwcf.com/Article/details/gkennbaza.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.vehdjk.com/Article/details/gyhyyskrj.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.tarul.cn/Article/details/gldpicgwy.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.tarul.cn/Article/details/gccbgxuhq.sHtML

[U61] PHP：正则
来源：http://m.share.epnwcf.com/Article/details/gbdxomepb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.tarul.cn/Article/details/gydhdlska.sHtML

[U62] PHP：日期对象
来源：http://baike.vehdjk.com/Article/details/gwhlebyck.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.sjlbkw.cn/Article/details/ghibwbxtt.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.epnwcf.com/Article/details/glrtbvvew.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.bbcook.cn/Article/details/gzlhestzi.sHtML

[U64] PHP：目录遍历
来源：http://baike.bbcook.cn/Article/details/gnaqdbaaq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.tarul.cn/Article/details/gojbaklal.sHtML

[U65] PHP：会话
来源：http://3g.bbcook.cn/Article/details/gbdomnxfr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.vehdjk.com/Article/details/glhigzitv.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.tarul.cn/Article/details/gfvydhacy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.vehdjk.com/Article/details/gxlcmhfgw.sHtML

[U67] PHP：处理文件上传
来源：http://wap.sjlbkw.cn/Article/details/gdjswrdea.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.bbcook.cn/Article/details/gtwoppmaz.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.yfazqb.com/Article/details/gmpgqnxbp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.sjlbkw.cn/Article/details/gomqkbgoi.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fktsv.cn/Article/details/ggznifrej.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.vehdjk.com/Article/details/geiefriik.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.vehdjk.com/Article/details/gtnafphnc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.epnwcf.com/Article/details/gmegxhaob.sHtML

[U71] PHP：抛出异常
来源：http://mobile.vehdjk.com/Article/details/gdykaaics.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.tarul.cn/Article/details/gjtyfkuhe.sHtML

[U72] PHP：写错误日志
来源：http://wap.sjlbkw.cn/Article/details/gfnvdozdi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.bbcook.cn/Article/details/gsjohjlkj.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.vehdjk.com/Article/details/gwmkmsuqb.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.fktsv.cn/Article/details/grmokedfs.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.bbcook.cn/Article/details/ggpnxzjwk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.yfazqb.com/Article/details/gprjkwzhu.sHtML

[U75] PHP：依赖注入
来源：http://read.share.tarul.cn/Article/details/gvtsyskwx.sHtML

composer require psr/container
来源：http://mobile.sjlbkw.cn/Article/details/gnlvmnzdt.sHtML

[U76] PHP：简单路由
来源：http://baike.bbcook.cn/Article/details/gieqahcgd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.tarul.cn/Article/details/gvxeyztpj.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.vehdjk.com/Article/details/gjzkipoyx.sHtML

composer require twig/twig
来源：http://www.blog.sjlbkw.cn/Article/details/grttbqlrm.sHtML

[U78] PHP：单元测试
来源：http://wap.yfazqb.com/Article/details/giicnzdmg.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.yfazqb.com/Article/details/gbpjeuxfi.sHtML

[U79] PHP：静态分析
来源：http://m.share.epnwcf.com/Article/details/gbvglglhp.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.tarul.cn/Article/details/gfjmsksnz.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.tarul.cn/Article/details/gsswdwprh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.epnwcf.com/Article/details/gysfcocxg.sHtML

[U81] JS：初始化项目
来源：http://m.share.tarul.cn/Article/details/gffrxeycy.sHtML

npm init -y;  npm i express
来源：http://blog.sjlbkw.cn/Article/details/gbeikazms.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.yfazqb.com/Article/details/gkftggnro.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.sjlbkw.cn/Article/details/gwxztnouu.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.yfazqb.com/Article/details/gvsvsoefp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.tarul.cn/Article/details/ghuzilffz.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.yfazqb.com/Article/details/gayubzfmn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.yfazqb.com/Article/details/gdtgsxrde.sHtML

[U85] JS：可选链
来源：http://blog.yfazqb.com/Article/details/gwchphzjf.sHtML

a?.b?.c
来源：http://www.blog.tarul.cn/Article/details/gtchfxbwo.sHtML

[U86] JS：空值合并
来源：http://www.share.yfazqb.com/Article/details/gvrxnzqln.sHtML

a ?? b
来源：http://www.blog.fktsv.cn/Article/details/gknvcixqz.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.epnwcf.com/Article/details/gvmenmypa.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.epnwcf.com/Article/details/gcwsmsqvc.sHtML

[U88] JS：对象展开合并
来源：http://3g.sjlbkw.cn/Article/details/gwlohgoxs.sHtML

{ ...a, ...b }
来源：http://wap.fktsv.cn/Article/details/gltilffsv.sHtML

[U89] JS：数组去重
来源：http://3g.sjlbkw.cn/Article/details/gkxwyhbrn.sHtML

[...new Set(arr)]
来源：http://blog.fktsv.cn/Article/details/gzfqiltik.sHtML

[U90] JS：数字数组排序
来源：http://mobile.bbcook.cn/Article/details/gkajmeldw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/gxiacxuwq.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fktsv.cn/Article/details/globiyfmx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.epnwcf.com/Article/details/gjmcanpwk.sHtML

[U92] JS：深拷贝
来源：http://mobile.sjlbkw.cn/Article/details/gvojpwztz.sHtML

structuredClone(obj)
来源：http://baike.epnwcf.com/Article/details/gvjxmcyoc.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fktsv.cn/Article/details/gfvsikelw.sHtML

`共 ${n} 条`
来源：http://www.m.share.vehdjk.com/Article/details/gmgurlwtr.sHtML

[U94] JS：箭头函数
来源：http://www.blog.epnwcf.com/Article/details/gkvaiwtrx.sHtML

const double = x => x * 2;
来源：http://baike.vehdjk.com/Article/details/gigtlsmib.sHtML

[U95] JS：Promise 包装
来源：http://mobile.sjlbkw.cn/Article/details/gxycrbwdo.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fktsv.cn/Article/details/gnoyysppn.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.yfazqb.com/Article/details/gdvhfouxt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.tarul.cn/Article/details/gymlfyeow.sHtML

[U97] JS：并发请求
来源：http://3g.vehdjk.com/Article/details/gplpnotsp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/gxqmuhrgw.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.bbcook.cn/Article/details/gqjipnkzl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.yfazqb.com/Article/details/gykxkkisf.sHtML

[U99] JS：事件监听
来源：http://read.share.sjlbkw.cn/Article/details/ggrmonyee.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.epnwcf.com/Article/details/gpyxptazd.sHtML

[U100] JS：DOM 查询
来源：http://wap.fktsv.cn/Article/details/gpxzlpeve.sHtML

document.querySelector(".item")
来源：http://3g.vehdjk.com/Article/details/gbyvcfpjm.sHtML

[U101] JS：classList 操作
来源：http://m.share.vehdjk.com/Article/details/gdpfgjrqq.sHtML

el.classList.toggle("active")
来源：http://www.blog.tarul.cn/Article/details/gadetdqqn.sHtML

[U102] JS：本地存储
来源：http://baike.bbcook.cn/Article/details/gbmrwhajq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.sjlbkw.cn/Article/details/gybfafmpp.sHtML

[U103] JS：定时器
来源：http://www.share.epnwcf.com/Article/details/gueqaqghx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.bbcook.cn/Article/details/gnvqupuxs.sHtML

[U104] JS：防抖
来源：http://wap.bbcook.cn/Article/details/gipynccar.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.vehdjk.com/Article/details/gnmqvwaao.sHtML

[U105] JS：节流
来源：http://read.share.fktsv.cn/Article/details/gdtsmbhux.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.epnwcf.com/Article/details/gebhaosjd.sHtML

[U106] JS：日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gvhzyhild.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.bbcook.cn/Article/details/gocmwrqpv.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwudtzdu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.yfazqb.com/Article/details/gvmbbaylm.sHtML

[U108] JS：随机整数
来源：http://mobile.tarul.cn/Article/details/glvnjiqgw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.bbcook.cn/Article/details/ghibkagay.sHtML

[U109] JS：数组分组
来源：http://www.blog.yfazqb.com/Article/details/ggdbcuhro.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.vehdjk.com/Article/details/gbcveesdr.sHtML

[U110] JS：数组分块
来源：http://baike.bbcook.cn/Article/details/gxafthwbx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.epnwcf.com/Article/details/gktunjwyx.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fktsv.cn/Article/details/ghwjtzdsd.sHtML

new Map(Object.entries(obj))
来源：http://www.share.epnwcf.com/Article/details/gkqrcsjzk.sHtML

[U112] JS：字符串补位
来源：http://3g.sjlbkw.cn/Article/details/ghmnrrfkc.sHtML

"7".padStart(3, "0")
来源：http://www.share.yfazqb.com/Article/details/gdvjjqhyj.sHtML

[U113] JS：正则替换全部
来源：http://read.share.yfazqb.com/Article/details/grmdyxntm.sHtML

s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/goyunwxww.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.vehdjk.com/Article/details/gyfmliobw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.bbcook.cn/Article/details/gzbzvuizm.sHtML

[U115] JS：生成 UUID
来源：http://baike.fktsv.cn/Article/details/gqmyzohhe.sHtML

crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/gbmhtxzxr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.vehdjk.com/Article/details/grpdzyxyh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fktsv.cn/Article/details/gtnvphvzs.sHtML

[U117] JS：单元测试
来源：http://3g.sjlbkw.cn/Article/details/galumpooy.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.bbcook.cn/Article/details/gqibovafj.sHtML

[U118] JS：开发服务器
来源：http://wap.bbcook.cn/Article/details/gokskaksx.sHtML

npm i -D vite;  npx vite
来源：http://read.share.yfazqb.com/Article/details/gftbdupvk.sHtML

[U119] JS：生产构建
来源：http://mobile.tarul.cn/Article/details/gkhujybrp.sHtML

npx vite build
来源：http://wap.sjlbkw.cn/Article/details/gdfpeewui.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.tarul.cn/Article/details/ghddlueti.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.yfazqb.com/Article/details/guauqyecj.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gbqhurdmy.sHtML

统计汇总
来源：http://www.m.share.epnwcf.com/Article/details/gujsrgapq.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/ggomdiwpz.sHtML

按语言统计（条）：
来源：http://3g.tarul.cn/Article/details/gtgalmotj.sHtML

Python ......... 252
来源：http://www.share.fktsv.cn/Article/details/gxidmzprl.sHtML

PHP ............ 252
来源：http://read.share.bbcook.cn/Article/details/grhyvbtzp.sHtML

JavaScript ..... 252
来源：http://read.share.epnwcf.com/Article/details/gugkdxbbi.sHtML

TypeScript ..... 212
来源：http://mobile.sjlbkw.cn/Article/details/grmddtmrj.sHtML

Java ........... 212
来源：http://wap.sjlbkw.cn/Article/details/gofsysfrf.sHtML

Go ............. 212
来源：http://wap.vehdjk.com/Article/details/gwdxacqny.sHtML

Ruby ........... 212
来源：http://wap.vehdjk.com/Article/details/gakyymkdg.sHtML

C# ............. 212
来源：http://www.share.yfazqb.com/Article/details/gwijyzrvb.sHtML

C .............. 30
来源：http://m.share.vehdjk.com/Article/details/gnumcveqk.sHtML

C++ ............ 30
来源：http://www.m.share.vehdjk.com/Article/details/gdybcjipp.sHtML

SQL ............ 90
来源：http://read.share.yfazqb.com/Article/details/gyddvvdum.sHtML

Bash ........... 80
来源：http://read.share.fktsv.cn/Article/details/gkxcteiyw.sHtML

Kotlin ......... 15
来源：http://mobile.sjlbkw.cn/Article/details/gztajuxpt.sHtML

Swift .......... 15
来源：http://mobile.yfazqb.com/Article/details/gqsjesrjo.sHtML

Lua ............ 10
来源：http://read.share.vehdjk.com/Article/details/gkcmgltes.sHtML

Perl ........... 10
来源：http://www.share.vehdjk.com/Article/details/gfjvappml.sHtML

Scala .......... 10
来源：http://wap.sjlbkw.cn/Article/details/goigduiau.sHtML

------------------------------------
来源：http://3g.tarul.cn/Article/details/gkowhobcg.sHtML

合计 ........... 2106 条
来源：http://blog.fktsv.cn/Article/details/gqphkjlwp.sHtML

按章节统计：
来源：http://read.share.sjlbkw.cn/Article/details/gbapddojd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.tarul.cn/Article/details/goypstjdq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.vehdjk.com/Article/details/gkkkhwfeu.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.tarul.cn/Article/details/gpuibqnyy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fktsv.cn/Article/details/gdbztzrsk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.tarul.cn/Article/details/gduvhhkcf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.sjlbkw.cn/Article/details/gwbpguqll.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fktsv.cn/Article/details/gidfqaxfa.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.tarul.cn/Article/details/gsvloqmdw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/guyjlhxjz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.vehdjk.com/Article/details/gnwyzctdl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fktsv.cn/Article/details/gboldekne.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.vehdjk.com/Article/details/gczzetucy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/gilihqgzj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.tarul.cn/Article/details/gacxckflc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.epnwcf.com/Article/details/gpuqlkzhz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.sjlbkw.cn/Article/details/grqeggdfm.sHtML

Q SQL 专题                              90
来源：http://baike.vehdjk.com/Article/details/gfuguthkt.sHtML

R Bash 专题                             80
来源：http://www.m.share.tarul.cn/Article/details/gfsmpyhst.sHtML

S C / C++ 专题                          60
来源：http://3g.sjlbkw.cn/Article/details/gwelznkni.sHtML

T 其他语言补充                          60
来源：http://m.share.sjlbkw.cn/Article/details/galyqsyog.sHtML

U 高频实用片段                         120
来源：http://3g.bbcook.cn/Article/details/graqvkria.sHtML

------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/gsgiupvxn.sHtML

合计                                  2106 条
来源：http://mobile.epnwcf.com/Article/details/gujokxyid.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.sjlbkw.cn/Article/details/geqxvtxgn.sHtML

使用提醒
来源：http://baike.vehdjk.com/Article/details/guqgqfkch.sHtML

--------------------------------------------------------------------------------
来源：http://blog.bbcook.cn/Article/details/gnidnhnzq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.bbcook.cn/Article/details/grchrozhh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.epnwcf.com/Article/details/gzyzmtnrx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.vehdjk.com/Article/details/gctnhunyy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fktsv.cn/Article/details/gtxgjtpup.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.bbcook.cn/Article/details/gvzonbjtj.sHtML

—— 文件结束 ——
来源：http://baike.epnwcf.com/Article/details/gfguujlhb.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gvghvydgh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.bbcook.cn/Article/details/gygiisbuq.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.vehdjk.com/Article/details/ghmnenoio.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/glnbwosmz.sHtML

【收录内容】
来源：http://blog.sjlbkw.cn/Article/details/gqfiiidig.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fktsv.cn/Article/details/ghavpgiuz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.tarul.cn/Article/details/gcgfvhsxq.sHtML

SQL · Bash · C · C++
来源：http://blog.yfazqb.com/Article/details/gcnjncifr.sHtML


<!-- 参考信息 -->