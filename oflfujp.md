代发 wailian999

[U03] Py：加载 .env 配置
来源：http://www.m.share.vehdjk.com/Article/details/gqbtxvmlg.sHtML

from dotenv import load_dotenv; load_dotenv()
来源：http://mobile.bbcook.cn/Article/details/gmpsbssxc.sHtML

[U04] Py：变量调试打印
来源：http://www.m.share.bbcook.cn/Article/details/gqlrdfxdn.sHtML

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mobile.tarul.cn/Article/details/gsreicbcx.sHtML

[U05] Py：列表去重且保序
来源：http://wap.sjlbkw.cn/Article/details/gtxyhhmyu.sHtML

list(dict.fromkeys(arr))
来源：http://www.share.sjlbkw.cn/Article/details/gvltgmxix.sHtML

[U06] Py：合并两个字典
来源：http://www.share.epnwcf.com/Article/details/gfgrrtevu.sHtML

{**a, **b}
来源：http://blog.vehdjk.com/Article/details/gscbxxoff.sHtML

[U07] Py：反转字典键值
来源：http://www.share.fktsv.cn/Article/details/gkrnnpvaf.sHtML

{v: k for k, v in d.items()}
来源：http://3g.vehdjk.com/Article/details/gimxhjebx.sHtML

[U08] Py：展平二维列表
来源：http://3g.sjlbkw.cn/Article/details/giedvfgmv.sHtML

[y for x in nested for y in x]
来源：http://www.blog.tarul.cn/Article/details/gtwmoowkm.sHtML

[U09] Py：字典取最大值的键
来源：http://blog.tarul.cn/Article/details/gdwctmlkv.sHtML

max(d, key=d.get)
来源：http://read.share.vehdjk.com/Article/details/gtytcimip.sHtML

[U10] Py：按值排序字典
来源：http://www.blog.yfazqb.com/Article/details/gxhvtjizr.sHtML

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.share.yfazqb.com/Article/details/gszvascmt.sHtML

[U11] Py：生成器表达式
来源：http://mobile.epnwcf.com/Article/details/gnzpjmktb.sHtML

(x * 2 for x in arr)
来源：http://www.share.vehdjk.com/Article/details/gsyjmcpyu.sHtML

[U12] Py：取出现最多的 3 个元素
来源：http://wap.vehdjk.com/Article/details/gmckfgvik.sHtML

Counter(arr).most_common(3)
来源：http://baike.fktsv.cn/Article/details/gkivimfld.sHtML

[U13] Py：固定长度队列
来源：http://www.m.share.fktsv.cn/Article/details/ghkifezku.sHtML

deque(maxlen=10)
来源：http://www.share.tarul.cn/Article/details/gouhijkab.sHtML

[U14] Py：分组收集到列表
来源：http://3g.vehdjk.com/Article/details/galjxxtom.sHtML

defaultdict(list)
来源：http://wap.vehdjk.com/Article/details/gyhtnhfcv.sHtML

[U15] Py：高精度计时
来源：http://blog.epnwcf.com/Article/details/gmabzvpov.sHtML

t = time.perf_counter()
来源：http://www.share.sjlbkw.cn/Article/details/goiqoobaa.sHtML

[U16] Py：命令行参数解析
来源：http://read.share.epnwcf.com/Article/details/gehjqpwja.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://blog.sjlbkw.cn/Article/details/goiraneiy.sHtML

[U17] Py：初始化日志
来源：http://www.blog.bbcook.cn/Article/details/gdxemhmqs.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://3g.vehdjk.com/Article/details/giqsrrwcy.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.tarul.cn/Article/details/gwhrqsfgo.sHtML

pat = re.compile(r"\d+")
来源：http://read.share.sjlbkw.cn/Article/details/grfmumoml.sHtML

[U19] Py：正则替换带回调
来源：http://www.share.sjlbkw.cn/Article/details/gjojahgyv.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wap.epnwcf.com/Article/details/gtjxshrho.sHtML

[U20] Py：缓存函数结果
来源：http://www.share.tarul.cn/Article/details/gsxgtbldx.sHtML

@functools.lru_cache(maxsize=None)
来源：http://mobile.epnwcf.com/Article/details/gvudarhhb.sHtML

[U21] Py：自定义上下文管理器
来源：http://www.blog.fktsv.cn/Article/details/gnezptfri.sHtML

@contextlib.contextmanager
来源：http://m.share.sjlbkw.cn/Article/details/gwerqwpfk.sHtML

[U22] Py：矩阵转置
来源：http://m.share.fktsv.cn/Article/details/ggfxsnmha.sHtML

list(zip(*m))
来源：http://wap.epnwcf.com/Article/details/gwbucujmg.sHtML

[U23] Py：分块读取大文件
来源：http://www.blog.sjlbkw.cn/Article/details/gmezkgcpe.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.share.yfazqb.com/Article/details/gqtdhppnl.sHtML

[U24] Py：路径操作
来源：http://read.share.fktsv.cn/Article/details/grzoonayg.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://m.share.vehdjk.com/Article/details/gzggckuxn.sHtML

[U25] Py：CSV 按字典读
来源：http://m.share.sjlbkw.cn/Article/details/gwlhtadrz.sHtML

csv.DictReader(f)
来源：http://m.share.yfazqb.com/Article/details/gpkskljzw.sHtML

[U26] Py：并发下载
来源：http://baike.vehdjk.com/Article/details/gsueseuwq.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://m.share.bbcook.cn/Article/details/geyzclmxv.sHtML

[U27] Py：异步 HTTP
来源：http://www.share.bbcook.cn/Article/details/gjgsdwpmr.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://3g.vehdjk.com/Article/details/gkjijichp.sHtML

[U28] Py：类型别名
来源：http://mobile.vehdjk.com/Article/details/ghvllxkjk.sHtML

UserId = int
来源：http://blog.sjlbkw.cn/Article/details/gtkceoxcv.sHtML

[U29] Py：属性校验
来源：http://blog.tarul.cn/Article/details/gvllklyta.sHtML

@property 与 @x.setter 配合
来源：http://www.share.epnwcf.com/Article/details/gkyjfkgsw.sHtML

[U30] Py：数据类
来源：http://www.m.share.epnwcf.com/Article/details/gxkowauca.sHtML

@dataclass(slots=True)
来源：http://www.m.share.tarul.cn/Article/details/guvreniru.sHtML

[U31] Py：单测
来源：http://baike.bbcook.cn/Article/details/gtvuhzfpw.sHtML

python -m pytest -q
来源：http://baike.bbcook.cn/Article/details/gduoyjvua.sHtML

[U32] Py：代码格式化
来源：http://baike.yfazqb.com/Article/details/gaxxlwpvk.sHtML

ruff format . && ruff check --fix .
来源：http://wap.yfazqb.com/Article/details/ggvqzqowo.sHtML

[U33] Py：打包发布
来源：http://www.m.share.vehdjk.com/Article/details/gvrsuotfj.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://m.share.epnwcf.com/Article/details/gyzaelgiz.sHtML

[U34] Py：判断编码
来源：http://www.m.share.vehdjk.com/Article/details/gybkbnjyj.sHtML

chardet.detect(raw)
来源：http://blog.epnwcf.com/Article/details/gaoxftero.sHtML

[U35] Py：发送邮件
来源：http://3g.epnwcf.com/Article/details/ghloecups.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wap.bbcook.cn/Article/details/ggaejpykw.sHtML

[U36] Py：定时任务
来源：http://m.share.yfazqb.com/Article/details/gloovjypo.sHtML

schedule.every(10).minutes.do(job)
来源：http://baike.fktsv.cn/Article/details/guqthztff.sHtML

[U37] Py：读写 Excel
来源：http://m.share.vehdjk.com/Article/details/gwfmyvcil.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://mobile.fktsv.cn/Article/details/gyodabfqy.sHtML

[U38] Py：获取脚本所在目录
来源：http://www.blog.epnwcf.com/Article/details/grxdxsjwq.sHtML

Path(__file__).resolve().parent
来源：http://m.share.fktsv.cn/Article/details/gndkumlzh.sHtML

[U39] Py：判断是否在交互环境
来源：http://m.share.sjlbkw.cn/Article/details/grrddjawt.sHtML

sys.stdout.isatty()
来源：http://read.share.bbcook.cn/Article/details/gyfogvxaq.sHtML

[U40] Py：打印到标准错误
来源：http://www.m.share.tarul.cn/Article/details/gdznsulci.sHtML

print("err", file=sys.stderr)
来源：http://baike.tarul.cn/Article/details/giegdbzyu.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://www.m.share.vehdjk.com/Article/details/gxfvuhrlo.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.vehdjk.com/Article/details/gnaxszbsd.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.bbcook.cn/Article/details/gfaudxdnt.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.bbcook.cn/Article/details/gyopzhxka.sHtML

[U43] PHP：声明命名空间
来源：http://www.m.share.sjlbkw.cn/Article/details/gzengvtwn.sHtML

namespace App\Http;
来源：http://read.share.sjlbkw.cn/Article/details/gqpazwkys.sHtML

[U44] PHP：开启严格类型
来源：http://wap.fktsv.cn/Article/details/goygljcti.sHtML

declare(strict_types=1);
来源：http://baike.sjlbkw.cn/Article/details/gqyzvlxzl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.tarul.cn/Article/details/ghnngvjxg.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.epnwcf.com/Article/details/gbushqblv.sHtML

[U46] PHP：可空类型
来源：http://blog.fktsv.cn/Article/details/gkkrwdfdh.sHtML

?string $name = null
来源：http://m.share.yfazqb.com/Article/details/gaqmktoyg.sHtML

[U47] PHP：联合类型
来源：http://3g.sjlbkw.cn/Article/details/gwhxmkwjz.sHtML

int|string $id
来源：http://wap.bbcook.cn/Article/details/gqsjvuxfa.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fktsv.cn/Article/details/getoatkiu.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.tarul.cn/Article/details/gnyjebgpq.sHtML

[U49] PHP：只读属性
来源：http://read.share.epnwcf.com/Article/details/gfawhhkha.sHtML

public readonly string $name
来源：http://wap.fktsv.cn/Article/details/ggvtyxlta.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.sjlbkw.cn/Article/details/gutmymdls.sHtML

public function __construct(private int $id) {}
来源：http://3g.vehdjk.com/Article/details/gdaeujlnh.sHtML

[U51] PHP：数组解构
来源：http://baike.fktsv.cn/Article/details/gtysefnpu.sHtML

[$a, $b] = $arr;
来源：http://blog.bbcook.cn/Article/details/gdqixarev.sHtML

[U52] PHP：箭头函数
来源：http://www.share.epnwcf.com/Article/details/giqevuhgd.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.vehdjk.com/Article/details/gfvggpjpi.sHtML

[U53] PHP：空合并运算符
来源：http://wap.vehdjk.com/Article/details/gmmxtucdn.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fktsv.cn/Article/details/gytnyssfd.sHtML

[U54] PHP：空安全调用
来源：http://wap.fktsv.cn/Article/details/gcrtyohrx.sHtML

$obj?->method()
来源：http://blog.yfazqb.com/Article/details/gxobclrhi.sHtML

[U55] PHP：match 表达式
来源：http://blog.sjlbkw.cn/Article/details/gbsgkulau.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.bbcook.cn/Article/details/ghparzbyh.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.fktsv.cn/Article/details/gnvbbqvol.sHtML

f(a: 1, b: 2)
来源：http://baike.sjlbkw.cn/Article/details/gznmkndlf.sHtML

[U57] PHP：字符串插值
来源：http://m.share.yfazqb.com/Article/details/gyhbzwabl.sHtML

"值: {$a}"
来源：http://www.blog.bbcook.cn/Article/details/gpofpvuqb.sHtML

[U58] PHP：数组三件套
来源：http://www.share.vehdjk.com/Article/details/ghvlndhev.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fktsv.cn/Article/details/gbvyoeniu.sHtML

[U59] PHP：自定义排序
来源：http://blog.tarul.cn/Article/details/guagctdne.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.tarul.cn/Article/details/ghihanvpg.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.tarul.cn/Article/details/gtsduncae.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.vehdjk.com/Article/details/gdnswoair.sHtML

[U61] PHP：正则
来源：http://read.share.tarul.cn/Article/details/gqaurbfnj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.tarul.cn/Article/details/gsaltvhmn.sHtML

[U62] PHP：日期对象
来源：http://wap.bbcook.cn/Article/details/ghnwwktve.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.yfazqb.com/Article/details/grtwvhlth.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.yfazqb.com/Article/details/gxadcjbos.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.vehdjk.com/Article/details/gnjnahpcl.sHtML

[U64] PHP：目录遍历
来源：http://read.share.bbcook.cn/Article/details/gdsatypyf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.tarul.cn/Article/details/ganisbefl.sHtML

[U65] PHP：会话
来源：http://baike.tarul.cn/Article/details/gdholxjmp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fktsv.cn/Article/details/ggshstvmz.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.yfazqb.com/Article/details/gxbxdbtcy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wap.fktsv.cn/Article/details/gbnnqfamu.sHtML

[U67] PHP：处理文件上传
来源：http://wap.vehdjk.com/Article/details/gklxovkdk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.epnwcf.com/Article/details/gevmudqdx.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.epnwcf.com/Article/details/gwnxemwnf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.vehdjk.com/Article/details/gxcqyfbms.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.epnwcf.com/Article/details/gvmocirce.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.sjlbkw.cn/Article/details/gfnesyecp.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fktsv.cn/Article/details/gyddmvjce.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.epnwcf.com/Article/details/gfknfobal.sHtML

[U71] PHP：抛出异常
来源：http://blog.sjlbkw.cn/Article/details/gtetttdpg.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.bbcook.cn/Article/details/gytbexqxn.sHtML

[U72] PHP：写错误日志
来源：http://blog.tarul.cn/Article/details/gupropcng.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.sjlbkw.cn/Article/details/glmsveahd.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.epnwcf.com/Article/details/growzhbrv.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.epnwcf.com/Article/details/gokqucgum.sHtML

[U74] PHP：读取环境变量
来源：http://wap.bbcook.cn/Article/details/gfnzypmwt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.epnwcf.com/Article/details/gfoenlhjd.sHtML

[U75] PHP：依赖注入
来源：http://3g.epnwcf.com/Article/details/gaxngmdfo.sHtML

composer require psr/container
来源：http://m.share.vehdjk.com/Article/details/gdwavzohb.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.bbcook.cn/Article/details/gqbnwolcu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.epnwcf.com/Article/details/gyaybfuzg.sHtML

[U77] PHP：模板渲染
来源：http://blog.epnwcf.com/Article/details/gyeuvhupa.sHtML

composer require twig/twig
来源：http://wap.fktsv.cn/Article/details/godlgnjue.sHtML

[U78] PHP：单元测试
来源：http://www.blog.yfazqb.com/Article/details/giqwvehhn.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.bbcook.cn/Article/details/gdurgqvic.sHtML

[U79] PHP：静态分析
来源：http://www.blog.vehdjk.com/Article/details/ghzkyytir.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.yfazqb.com/Article/details/gvhgsmwka.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.sjlbkw.cn/Article/details/guxlmaclx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.sjlbkw.cn/Article/details/ghhkboguy.sHtML

[U81] JS：初始化项目
来源：http://wap.fktsv.cn/Article/details/gkntnkmuv.sHtML

npm init -y;  npm i express
来源：http://mobile.vehdjk.com/Article/details/gxzyerjzx.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.yfazqb.com/Article/details/gudcgaxhb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.yfazqb.com/Article/details/gslddkjhl.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.yfazqb.com/Article/details/guktbucjp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.fktsv.cn/Article/details/gpkrnwand.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fktsv.cn/Article/details/gxrieecqm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.yfazqb.com/Article/details/gdzbgwamb.sHtML

[U85] JS：可选链
来源：http://m.share.tarul.cn/Article/details/gbgvottss.sHtML

a?.b?.c
来源：http://wap.bbcook.cn/Article/details/gyfzvjtqi.sHtML

[U86] JS：空值合并
来源：http://www.share.fktsv.cn/Article/details/gxvsjddtt.sHtML

a ?? b
来源：http://www.m.share.bbcook.cn/Article/details/gtacznqsq.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.epnwcf.com/Article/details/gsvmzfxoe.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fktsv.cn/Article/details/gbxubwluo.sHtML

[U88] JS：对象展开合并
来源：http://read.share.vehdjk.com/Article/details/gvdnrnkwh.sHtML

{ ...a, ...b }
来源：http://blog.epnwcf.com/Article/details/gyslnuexr.sHtML

[U89] JS：数组去重
来源：http://www.share.epnwcf.com/Article/details/gqopcxumt.sHtML

[...new Set(arr)]
来源：http://www.share.fktsv.cn/Article/details/gdadsnzpi.sHtML

[U90] JS：数字数组排序
来源：http://read.share.sjlbkw.cn/Article/details/gdvauantp.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.tarul.cn/Article/details/guabkhvcd.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.tarul.cn/Article/details/glvwbovzn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.vehdjk.com/Article/details/gnbwxgjcn.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.yfazqb.com/Article/details/gltbwytrq.sHtML

structuredClone(obj)
来源：http://3g.bbcook.cn/Article/details/gshlyjfic.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.vehdjk.com/Article/details/gjndaogtz.sHtML

`共 ${n} 条`
来源：http://baike.epnwcf.com/Article/details/ghmjrzlgg.sHtML

[U94] JS：箭头函数
来源：http://wap.yfazqb.com/Article/details/grnhtjwnu.sHtML

const double = x => x * 2;
来源：http://www.blog.yfazqb.com/Article/details/gbhdtbdlf.sHtML

[U95] JS：Promise 包装
来源：http://www.share.yfazqb.com/Article/details/gtruwnihv.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.tarul.cn/Article/details/grhvgcpug.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.tarul.cn/Article/details/gueyfnzox.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.epnwcf.com/Article/details/gtdyrsjod.sHtML

[U97] JS：并发请求
来源：http://baike.bbcook.cn/Article/details/gbvnljjkm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.epnwcf.com/Article/details/gvjjlvqdo.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.yfazqb.com/Article/details/gjtuwitzc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.epnwcf.com/Article/details/gwxmqufjr.sHtML

[U99] JS：事件监听
来源：http://baike.tarul.cn/Article/details/gefmhsopn.sHtML

el.addEventListener("click", e => {})
来源：http://3g.tarul.cn/Article/details/ggcatwbrd.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.vehdjk.com/Article/details/gdvucrtzh.sHtML

document.querySelector(".item")
来源：http://m.share.epnwcf.com/Article/details/gizfqxypn.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.bbcook.cn/Article/details/gmylwkrty.sHtML

el.classList.toggle("active")
来源：http://read.share.vehdjk.com/Article/details/gctauudhp.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fktsv.cn/Article/details/gcgfnhioy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.sjlbkw.cn/Article/details/gtzxezmen.sHtML

[U103] JS：定时器
来源：http://m.share.sjlbkw.cn/Article/details/gmlyliddq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.bbcook.cn/Article/details/gghsokqoj.sHtML

[U104] JS：防抖
来源：http://mobile.yfazqb.com/Article/details/gmcuthwkq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/gumvxkalm.sHtML

[U105] JS：节流
来源：http://www.share.sjlbkw.cn/Article/details/guikjcfhs.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.tarul.cn/Article/details/gnnfgvawd.sHtML

[U106] JS：日期格式化
来源：http://read.share.epnwcf.com/Article/details/gigaerfvd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.tarul.cn/Article/details/gdraeybby.sHtML

[U107] JS：数字千分位
来源：http://3g.epnwcf.com/Article/details/gtqwrbiuo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.sjlbkw.cn/Article/details/gfckacmnl.sHtML

[U108] JS：随机整数
来源：http://wap.epnwcf.com/Article/details/gzwbvdjhb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.bbcook.cn/Article/details/gfzwhtnkg.sHtML

[U109] JS：数组分组
来源：http://read.share.vehdjk.com/Article/details/ggcwfoypt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.epnwcf.com/Article/details/gqadpxdkn.sHtML

[U110] JS：数组分块
来源：http://wap.vehdjk.com/Article/details/gtodujpey.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.bbcook.cn/Article/details/gixrrfbvu.sHtML

[U111] JS：对象转 Map
来源：http://3g.tarul.cn/Article/details/gigbncadl.sHtML

new Map(Object.entries(obj))
来源：http://3g.vehdjk.com/Article/details/gfaoheppu.sHtML

[U112] JS：字符串补位
来源：http://m.share.tarul.cn/Article/details/gqazuyrcr.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.bbcook.cn/Article/details/gxkgszahg.sHtML

[U113] JS：正则替换全部
来源：http://m.share.sjlbkw.cn/Article/details/gkwolpkpw.sHtML

s.replaceAll("a", "b")
来源：http://blog.epnwcf.com/Article/details/grviuayzm.sHtML

[U114] JS：JSON 深比较
来源：http://wap.bbcook.cn/Article/details/gtjywjrab.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.epnwcf.com/Article/details/gddytdsdu.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/ggakoyzyx.sHtML

crypto.randomUUID()
来源：http://baike.sjlbkw.cn/Article/details/gqoagsikf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.epnwcf.com/Article/details/grsexfykq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.vehdjk.com/Article/details/gqpacybzn.sHtML

[U117] JS：单元测试
来源：http://3g.sjlbkw.cn/Article/details/gdvaarqdr.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.epnwcf.com/Article/details/ggloyswmd.sHtML

[U118] JS：开发服务器
来源：http://www.share.epnwcf.com/Article/details/gczlhjiak.sHtML

npm i -D vite;  npx vite
来源：http://3g.bbcook.cn/Article/details/gxczifhcr.sHtML

[U119] JS：生产构建
来源：http://www.blog.epnwcf.com/Article/details/ghqnsnpdz.sHtML

npx vite build
来源：http://baike.yfazqb.com/Article/details/gvdgszmqd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fktsv.cn/Article/details/gpftkofga.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fktsv.cn/Article/details/ggnsfmsxm.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gzwsecbaq.sHtML

统计汇总
来源：http://read.share.tarul.cn/Article/details/gksstkmfx.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gryjhaqfa.sHtML

按语言统计（条）：
来源：http://www.share.tarul.cn/Article/details/gfollcnwz.sHtML

Python ......... 252
来源：http://blog.yfazqb.com/Article/details/guhgtogkv.sHtML

PHP ............ 252
来源：http://www.m.share.yfazqb.com/Article/details/gqovjpgwk.sHtML

JavaScript ..... 252
来源：http://baike.bbcook.cn/Article/details/gdomdrxig.sHtML

TypeScript ..... 212
来源：http://m.share.fktsv.cn/Article/details/gsprfnaqy.sHtML

Java ........... 212
来源：http://baike.fktsv.cn/Article/details/gklkcoifp.sHtML

Go ............. 212
来源：http://m.share.sjlbkw.cn/Article/details/gqquncmop.sHtML

Ruby ........... 212
来源：http://mobile.sjlbkw.cn/Article/details/gebuaiqxg.sHtML

C# ............. 212
来源：http://blog.vehdjk.com/Article/details/gqyezipbd.sHtML

C .............. 30
来源：http://3g.vehdjk.com/Article/details/gphgsbrci.sHtML

C++ ............ 30
来源：http://www.share.sjlbkw.cn/Article/details/gmcrhueev.sHtML

SQL ............ 90
来源：http://blog.tarul.cn/Article/details/gvozpglwq.sHtML

Bash ........... 80
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqdknpte.sHtML

Kotlin ......... 15
来源：http://wap.epnwcf.com/Article/details/gchtsasoq.sHtML

Swift .......... 15
来源：http://baike.tarul.cn/Article/details/gztomdsyi.sHtML

Lua ............ 10
来源：http://blog.yfazqb.com/Article/details/gntchwtsp.sHtML

Perl ........... 10
来源：http://3g.tarul.cn/Article/details/gjvhxiwmc.sHtML

Scala .......... 10
来源：http://www.m.share.fktsv.cn/Article/details/gpsbtncfv.sHtML

------------------------------------
来源：http://baike.fktsv.cn/Article/details/gudliuvlr.sHtML

合计 ........... 2106 条
来源：http://wap.vehdjk.com/Article/details/gsyzqfhax.sHtML

按章节统计：
来源：http://m.share.tarul.cn/Article/details/gntlwanih.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.epnwcf.com/Article/details/ggsoplesu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.vehdjk.com/Article/details/gtqxlkokm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.vehdjk.com/Article/details/gxtaltzwq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fktsv.cn/Article/details/gecrfibln.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.epnwcf.com/Article/details/gkapdzgpu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.epnwcf.com/Article/details/gnzoxagmi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.sjlbkw.cn/Article/details/goxntpoid.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.tarul.cn/Article/details/gbemlefju.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gvsblhcrx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.yfazqb.com/Article/details/glgoyzmar.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/gnwvtwgqc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.tarul.cn/Article/details/gpvgsjawq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/gckpnpjyb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.bbcook.cn/Article/details/gyoudisau.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.epnwcf.com/Article/details/gazqrmjeb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fktsv.cn/Article/details/gckrhbvck.sHtML

Q SQL 专题                              90
来源：http://3g.vehdjk.com/Article/details/gxbzwfupa.sHtML

R Bash 专题                             80
来源：http://baike.sjlbkw.cn/Article/details/grszqdmdn.sHtML

S C / C++ 专题                          60
来源：http://wap.yfazqb.com/Article/details/gegavqlqx.sHtML

T 其他语言补充                          60
来源：http://mobile.yfazqb.com/Article/details/godckuzrb.sHtML

U 高频实用片段                         120
来源：http://www.m.share.tarul.cn/Article/details/grycskpcb.sHtML

------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/gnfpeugel.sHtML

合计                                  2106 条
来源：http://mobile.sjlbkw.cn/Article/details/ggewqfmet.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.bbcook.cn/Article/details/gdvivsfrq.sHtML

使用提醒
来源：http://mobile.fktsv.cn/Article/details/grywsnmpf.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gaqnzgsmy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.bbcook.cn/Article/details/gkokmrhei.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.sjlbkw.cn/Article/details/grqmqziho.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fktsv.cn/Article/details/gmjydnyhf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.epnwcf.com/Article/details/ggnndarvb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.yfazqb.com/Article/details/gtlhkuagd.sHtML

—— 文件结束 ——
来源：http://3g.sjlbkw.cn/Article/details/guutnryhs.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gsuffvkzf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.vehdjk.com/Article/details/groaeliuw.sHtML

Common Programming Examples Cheat Book
来源：http://3g.sjlbkw.cn/Article/details/gycvtgyor.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gtuokbfco.sHtML

【收录内容】
来源：http://www.blog.sjlbkw.cn/Article/details/grcizmaql.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.bbcook.cn/Article/details/gpglmygcw.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.sjlbkw.cn/Article/details/gqnfkkjbn.sHtML

SQL · Bash · C · C++
来源：http://mobile.fktsv.cn/Article/details/gvfneyqwa.sHtML


<!-- 参考信息 -->