代发 wailian999

[U13] Py：固定长度队列
来源：http://mobile.bbcook.cn/Article/details/gkjesqrxk.sHtML

deque(maxlen=10)
来源：http://read.share.sjlbkw.cn/Article/details/gfhqswugd.sHtML

[U14] Py：分组收集到列表
来源：http://www.m.share.tarul.cn/Article/details/ghzlojxue.sHtML

defaultdict(list)
来源：http://mobile.bbcook.cn/Article/details/ggrzgeswx.sHtML

[U15] Py：高精度计时
来源：http://m.share.epnwcf.com/Article/details/ghatbiawk.sHtML

t = time.perf_counter()
来源：http://wap.bbcook.cn/Article/details/gfxmolpfa.sHtML

[U16] Py：命令行参数解析
来源：http://baike.yfazqb.com/Article/details/gtdggrfms.sHtML

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.blog.tarul.cn/Article/details/gzurgcroo.sHtML

[U17] Py：初始化日志
来源：http://read.share.epnwcf.com/Article/details/gfxcozxtv.sHtML

logging.basicConfig(level=logging.INFO)
来源：http://mobile.fktsv.cn/Article/details/ggvglytld.sHtML

[U18] Py：预编译正则
来源：http://www.m.share.yfazqb.com/Article/details/gxvqxuomi.sHtML

pat = re.compile(r"\d+")
来源：http://baike.tarul.cn/Article/details/gijsqwvnz.sHtML

[U19] Py：正则替换带回调
来源：http://www.m.share.bbcook.cn/Article/details/ghxzcdcpc.sHtML

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blog.epnwcf.com/Article/details/gzrhpezvs.sHtML

[U20] Py：缓存函数结果
来源：http://www.blog.yfazqb.com/Article/details/gkqkkqpun.sHtML

@functools.lru_cache(maxsize=None)
来源：http://www.blog.vehdjk.com/Article/details/geocrboeu.sHtML

[U21] Py：自定义上下文管理器
来源：http://mobile.vehdjk.com/Article/details/gwrfaptcw.sHtML

@contextlib.contextmanager
来源：http://mobile.tarul.cn/Article/details/gpvcpmber.sHtML

[U22] Py：矩阵转置
来源：http://www.share.yfazqb.com/Article/details/gqkwlxrbu.sHtML

list(zip(*m))
来源：http://www.m.share.yfazqb.com/Article/details/gawdgdyca.sHtML

[U23] Py：分块读取大文件
来源：http://read.share.epnwcf.com/Article/details/gewylbxbd.sHtML

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqxmquqo.sHtML

[U24] Py：路径操作
来源：http://www.m.share.tarul.cn/Article/details/gfnaugsks.sHtML

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://blog.bbcook.cn/Article/details/gzcwougzz.sHtML

[U25] Py：CSV 按字典读
来源：http://read.share.epnwcf.com/Article/details/gxglnsfco.sHtML

csv.DictReader(f)
来源：http://www.m.share.tarul.cn/Article/details/gvrnhnmkk.sHtML

[U26] Py：并发下载
来源：http://www.blog.epnwcf.com/Article/details/gucfqprlj.sHtML

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mobile.bbcook.cn/Article/details/ghuvsxlrn.sHtML

[U27] Py：异步 HTTP
来源：http://wap.vehdjk.com/Article/details/grqgshnrj.sHtML

aiohttp.ClientSession() 配合 async with
来源：http://blog.sjlbkw.cn/Article/details/gcydnxrha.sHtML

[U28] Py：类型别名
来源：http://baike.yfazqb.com/Article/details/ghtedsyzb.sHtML

UserId = int
来源：http://wap.fktsv.cn/Article/details/gxnxcngma.sHtML

[U29] Py：属性校验
来源：http://read.share.yfazqb.com/Article/details/gldagcsan.sHtML

@property 与 @x.setter 配合
来源：http://www.m.share.tarul.cn/Article/details/gitvzvzex.sHtML

[U30] Py：数据类
来源：http://blog.bbcook.cn/Article/details/gbrlhlzbb.sHtML

@dataclass(slots=True)
来源：http://www.blog.fktsv.cn/Article/details/gepamgxrg.sHtML

[U31] Py：单测
来源：http://www.share.tarul.cn/Article/details/gxgxzidhj.sHtML

python -m pytest -q
来源：http://read.share.epnwcf.com/Article/details/gnhoodeig.sHtML

[U32] Py：代码格式化
来源：http://wap.sjlbkw.cn/Article/details/ghcmbkvtp.sHtML

ruff format . && ruff check --fix .
来源：http://www.m.share.bbcook.cn/Article/details/gxnernnah.sHtML

[U33] Py：打包发布
来源：http://mobile.tarul.cn/Article/details/grlmwozzc.sHtML

python -m build  （依赖 pyproject.toml）
来源：http://wap.bbcook.cn/Article/details/gvbowzthl.sHtML

[U34] Py：判断编码
来源：http://www.m.share.sjlbkw.cn/Article/details/gguzzdwtr.sHtML

chardet.detect(raw)
来源：http://baike.yfazqb.com/Article/details/gahsxplqq.sHtML

[U35] Py：发送邮件
来源：http://www.share.vehdjk.com/Article/details/gqqwqezbr.sHtML

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://read.share.epnwcf.com/Article/details/gyzuraerm.sHtML

[U36] Py：定时任务
来源：http://wap.bbcook.cn/Article/details/gpzsabvya.sHtML

schedule.every(10).minutes.do(job)
来源：http://mobile.yfazqb.com/Article/details/gbogvjuhp.sHtML

[U37] Py：读写 Excel
来源：http://www.blog.bbcook.cn/Article/details/gwrxpcizf.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://3g.vehdjk.com/Article/details/gkzutgyvx.sHtML

[U38] Py：获取脚本所在目录
来源：http://baike.epnwcf.com/Article/details/goiwjgmzc.sHtML

Path(__file__).resolve().parent
来源：http://3g.sjlbkw.cn/Article/details/gsicdkjyq.sHtML

[U39] Py：判断是否在交互环境
来源：http://www.blog.tarul.cn/Article/details/gzujepjou.sHtML

sys.stdout.isatty()
来源：http://3g.vehdjk.com/Article/details/gotugwqko.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.yfazqb.com/Article/details/gvbeydjsn.sHtML

print("err", file=sys.stderr)
来源：http://wap.vehdjk.com/Article/details/gncsxsgta.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.fktsv.cn/Article/details/gxhjgowov.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.bbcook.cn/Article/details/gwavsnrat.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://baike.yfazqb.com/Article/details/gvhejawzm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.m.share.bbcook.cn/Article/details/gexlyhwnt.sHtML

[U43] PHP：声明命名空间
来源：http://baike.vehdjk.com/Article/details/gmfpqvplm.sHtML

namespace App\Http;
来源：http://www.share.fktsv.cn/Article/details/gpwyjhuzn.sHtML

[U44] PHP：开启严格类型
来源：http://mobile.fktsv.cn/Article/details/ghirvkdax.sHtML

declare(strict_types=1);
来源：http://blog.epnwcf.com/Article/details/gimvgssgx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://mobile.fktsv.cn/Article/details/gyyovwwoh.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.epnwcf.com/Article/details/gbszkpbtr.sHtML

[U46] PHP：可空类型
来源：http://3g.vehdjk.com/Article/details/glnqscbsl.sHtML

?string $name = null
来源：http://www.share.epnwcf.com/Article/details/gcqzuwyai.sHtML

[U47] PHP：联合类型
来源：http://wap.vehdjk.com/Article/details/gycthiasb.sHtML

int|string $id
来源：http://wap.vehdjk.com/Article/details/gyjdovfeq.sHtML

[U48] PHP：纯枚举
来源：http://www.share.yfazqb.com/Article/details/ghyiqpiid.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://read.share.sjlbkw.cn/Article/details/gunmoljxc.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.bbcook.cn/Article/details/gaioffljw.sHtML

public readonly string $name
来源：http://www.m.share.vehdjk.com/Article/details/gowngalbs.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.sjlbkw.cn/Article/details/gznzwehit.sHtML

public function __construct(private int $id) {}
来源：http://baike.yfazqb.com/Article/details/gietykuqi.sHtML

[U51] PHP：数组解构
来源：http://wap.yfazqb.com/Article/details/gefcsaexu.sHtML

[$a, $b] = $arr;
来源：http://mobile.fktsv.cn/Article/details/gptiozcob.sHtML

[U52] PHP：箭头函数
来源：http://mobile.epnwcf.com/Article/details/gwysnzbtc.sHtML

$double = fn($x) => $x * 2;
来源：http://blog.epnwcf.com/Article/details/gxptragzf.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.tarul.cn/Article/details/ghmtrfajn.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.bbcook.cn/Article/details/ghdliytog.sHtML

[U54] PHP：空安全调用
来源：http://3g.epnwcf.com/Article/details/gqvzrdudt.sHtML

$obj?->method()
来源：http://wap.tarul.cn/Article/details/gmgvqjyqj.sHtML

[U55] PHP：match 表达式
来源：http://mobile.tarul.cn/Article/details/gdcfckgxi.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.vehdjk.com/Article/details/gthfquzyh.sHtML

[U56] PHP：命名参数
来源：http://baike.epnwcf.com/Article/details/gpnapnbih.sHtML

f(a: 1, b: 2)
来源：http://www.share.bbcook.cn/Article/details/gnaiuiivn.sHtML

[U57] PHP：字符串插值
来源：http://m.share.bbcook.cn/Article/details/gkmwkxufj.sHtML

"值: {$a}"
来源：http://read.share.epnwcf.com/Article/details/gvyibtcae.sHtML

[U58] PHP：数组三件套
来源：http://wap.tarul.cn/Article/details/gqgerrips.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.sjlbkw.cn/Article/details/gsxljehzy.sHtML

[U59] PHP：自定义排序
来源：http://m.share.sjlbkw.cn/Article/details/gvodltkzz.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.vehdjk.com/Article/details/ggnvlvnob.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.sjlbkw.cn/Article/details/gcmjwrsgx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.yfazqb.com/Article/details/gnwbnwxmz.sHtML

[U61] PHP：正则
来源：http://baike.bbcook.cn/Article/details/gicwsakqx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.epnwcf.com/Article/details/ghoztkhbl.sHtML

[U62] PHP：日期对象
来源：http://wap.sjlbkw.cn/Article/details/glqoyqnbb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.fktsv.cn/Article/details/gsrazxgum.sHtML

[U63] PHP：文件读写
来源：http://blog.epnwcf.com/Article/details/glolcqgxs.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.yfazqb.com/Article/details/gadgbfmds.sHtML

[U64] PHP：目录遍历
来源：http://m.share.sjlbkw.cn/Article/details/giesnnvfk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.epnwcf.com/Article/details/gnyzhdgxu.sHtML

[U65] PHP：会话
来源：http://mobile.sjlbkw.cn/Article/details/gpjfbttpm.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.tarul.cn/Article/details/gwdxyguyg.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.fktsv.cn/Article/details/gbevdknkg.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.epnwcf.com/Article/details/gphoxcajg.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.sjlbkw.cn/Article/details/grdqhipqs.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.vehdjk.com/Article/details/gtamjbfri.sHtML

[U68] PHP：PDO 连接
来源：http://blog.tarul.cn/Article/details/goslkrbik.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.tarul.cn/Article/details/gaxdrosdr.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.epnwcf.com/Article/details/gjzlnlbio.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.yfazqb.com/Article/details/gnqeuwlax.sHtML

[U70] PHP：PDO 事务
来源：http://baike.yfazqb.com/Article/details/gamirkvmc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.epnwcf.com/Article/details/gdrvvdhmh.sHtML

[U71] PHP：抛出异常
来源：http://3g.sjlbkw.cn/Article/details/gkjuxvkmj.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.sjlbkw.cn/Article/details/gpqtqxeym.sHtML

[U72] PHP：写错误日志
来源：http://baike.sjlbkw.cn/Article/details/gjxercsff.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fktsv.cn/Article/details/gtmcrcnvz.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.epnwcf.com/Article/details/gorctpjbj.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.bbcook.cn/Article/details/gfngddhtq.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fktsv.cn/Article/details/gkvzoqfvx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.epnwcf.com/Article/details/gkgbfunvb.sHtML

[U75] PHP：依赖注入
来源：http://wap.epnwcf.com/Article/details/gdxcwcrzl.sHtML

composer require psr/container
来源：http://read.share.tarul.cn/Article/details/gvoqhgqfx.sHtML

[U76] PHP：简单路由
来源：http://wap.vehdjk.com/Article/details/gfqigecqd.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.epnwcf.com/Article/details/gbolcylef.sHtML

[U77] PHP：模板渲染
来源：http://m.share.bbcook.cn/Article/details/gkubgeasz.sHtML

composer require twig/twig
来源：http://www.share.bbcook.cn/Article/details/gmirpcogc.sHtML

[U78] PHP：单元测试
来源：http://wap.yfazqb.com/Article/details/gvbsuiqha.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.vehdjk.com/Article/details/gxjbjjlzf.sHtML

[U79] PHP：静态分析
来源：http://m.share.fktsv.cn/Article/details/gisvomkdu.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.yfazqb.com/Article/details/gcrwgtstr.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fktsv.cn/Article/details/gszchkfzi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.epnwcf.com/Article/details/glslwkzsg.sHtML

[U81] JS：初始化项目
来源：http://wap.yfazqb.com/Article/details/gkjcuhnzf.sHtML

npm init -y;  npm i express
来源：http://mobile.epnwcf.com/Article/details/gsepxmlnb.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.yfazqb.com/Article/details/goihfljic.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.tarul.cn/Article/details/ggnvfgnhc.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnhcwmrx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.sjlbkw.cn/Article/details/gkpqzupau.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fktsv.cn/Article/details/ggfdufudk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.bbcook.cn/Article/details/gcgdygzzd.sHtML

[U85] JS：可选链
来源：http://www.m.share.tarul.cn/Article/details/gkuwmmspc.sHtML

a?.b?.c
来源：http://wap.fktsv.cn/Article/details/gisefjsny.sHtML

[U86] JS：空值合并
来源：http://mobile.yfazqb.com/Article/details/gywojzwsj.sHtML

a ?? b
来源：http://www.share.epnwcf.com/Article/details/gsfsvejby.sHtML

[U87] JS：解构默认值
来源：http://blog.vehdjk.com/Article/details/gawsrhsqt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.tarul.cn/Article/details/gumshfjrc.sHtML

[U88] JS：对象展开合并
来源：http://3g.fktsv.cn/Article/details/gbegjukho.sHtML

{ ...a, ...b }
来源：http://blog.yfazqb.com/Article/details/gmsznhlyn.sHtML

[U89] JS：数组去重
来源：http://mobile.yfazqb.com/Article/details/gjzgwjvki.sHtML

[...new Set(arr)]
来源：http://mobile.bbcook.cn/Article/details/gpljdtrrv.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.epnwcf.com/Article/details/ghuuwtxuf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/gzjelvgvb.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fktsv.cn/Article/details/gosvviblp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.yfazqb.com/Article/details/gwkxdvnqz.sHtML

[U92] JS：深拷贝
来源：http://baike.epnwcf.com/Article/details/gbbxjolgv.sHtML

structuredClone(obj)
来源：http://blog.tarul.cn/Article/details/gelvapmrh.sHtML

[U93] JS：模板字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gpnnjgdzq.sHtML

`共 ${n} 条`
来源：http://3g.tarul.cn/Article/details/ghvvgodbt.sHtML

[U94] JS：箭头函数
来源：http://blog.sjlbkw.cn/Article/details/gvibjlgca.sHtML

const double = x => x * 2;
来源：http://baike.vehdjk.com/Article/details/gtjggpgva.sHtML

[U95] JS：Promise 包装
来源：http://www.share.vehdjk.com/Article/details/gbmcswmcc.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.tarul.cn/Article/details/gpyrexqcd.sHtML

[U96] JS：async/await 与异常
来源：http://baike.epnwcf.com/Article/details/gsgjdwgme.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fktsv.cn/Article/details/gdhwehgoz.sHtML

[U97] JS：并发请求
来源：http://www.m.share.tarul.cn/Article/details/gwgvgwkdk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gvfmsghvm.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.yfazqb.com/Article/details/gjmrpljrb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.bbcook.cn/Article/details/gmcsckbil.sHtML

[U99] JS：事件监听
来源：http://mobile.sjlbkw.cn/Article/details/gajcdsuin.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.yfazqb.com/Article/details/gbbjoqnba.sHtML

[U100] JS：DOM 查询
来源：http://mobile.sjlbkw.cn/Article/details/gfapmwpgk.sHtML

document.querySelector(".item")
来源：http://www.share.fktsv.cn/Article/details/gmeihkwcv.sHtML

[U101] JS：classList 操作
来源：http://wap.yfazqb.com/Article/details/gsqqmevqa.sHtML

el.classList.toggle("active")
来源：http://m.share.tarul.cn/Article/details/giqjhqtjy.sHtML

[U102] JS：本地存储
来源：http://mobile.vehdjk.com/Article/details/gttutymma.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.vehdjk.com/Article/details/gkckmplbl.sHtML

[U103] JS：定时器
来源：http://read.share.vehdjk.com/Article/details/gamfprgnt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.epnwcf.com/Article/details/gfnrtpslp.sHtML

[U104] JS：防抖
来源：http://www.m.share.bbcook.cn/Article/details/gyulnrvto.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fktsv.cn/Article/details/gbepxcwnq.sHtML

[U105] JS：节流
来源：http://blog.sjlbkw.cn/Article/details/gflhwhwjv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.vehdjk.com/Article/details/gyqgbotot.sHtML

[U106] JS：日期格式化
来源：http://blog.vehdjk.com/Article/details/gxsxgpspm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.tarul.cn/Article/details/gqfysjwkn.sHtML

[U107] JS：数字千分位
来源：http://m.share.bbcook.cn/Article/details/gqsgzlukv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.vehdjk.com/Article/details/gpbdzwldj.sHtML

[U108] JS：随机整数
来源：http://www.m.share.tarul.cn/Article/details/gdcwteome.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.tarul.cn/Article/details/gdpxwvenf.sHtML

[U109] JS：数组分组
来源：http://m.share.yfazqb.com/Article/details/garcwsoni.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.bbcook.cn/Article/details/getcjbhre.sHtML

[U110] JS：数组分块
来源：http://blog.vehdjk.com/Article/details/gwrwohnma.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fktsv.cn/Article/details/gcrkujjlz.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.vehdjk.com/Article/details/gmguelkvt.sHtML

new Map(Object.entries(obj))
来源：http://mobile.sjlbkw.cn/Article/details/gmetyrdai.sHtML

[U112] JS：字符串补位
来源：http://wap.fktsv.cn/Article/details/guahmwfra.sHtML

"7".padStart(3, "0")
来源：http://blog.fktsv.cn/Article/details/gwsysegtr.sHtML

[U113] JS：正则替换全部
来源：http://read.share.tarul.cn/Article/details/ghcmhxzbb.sHtML

s.replaceAll("a", "b")
来源：http://mobile.epnwcf.com/Article/details/ggvqyuwkb.sHtML

[U114] JS：JSON 深比较
来源：http://wap.epnwcf.com/Article/details/gjqriccbq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.yfazqb.com/Article/details/ghujxhkgm.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.tarul.cn/Article/details/gotgadhfn.sHtML

crypto.randomUUID()
来源：http://www.m.share.bbcook.cn/Article/details/gryfcozbv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.yfazqb.com/Article/details/ggoxmedys.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.epnwcf.com/Article/details/gkgpndzge.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fktsv.cn/Article/details/gkbyaecnk.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.epnwcf.com/Article/details/gafqaiqej.sHtML

[U118] JS：开发服务器
来源：http://wap.epnwcf.com/Article/details/gkaktvcfm.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.bbcook.cn/Article/details/gvwcnymuk.sHtML

[U119] JS：生产构建
来源：http://baike.fktsv.cn/Article/details/gdhzirnev.sHtML

npx vite build
来源：http://wap.vehdjk.com/Article/details/gbztbqoyj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.sjlbkw.cn/Article/details/grcupgqil.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.tarul.cn/Article/details/gzakitaul.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gwdbxnzjj.sHtML

统计汇总
来源：http://blog.tarul.cn/Article/details/gmxiqoyfl.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gcslosmxb.sHtML

按语言统计（条）：
来源：http://mobile.vehdjk.com/Article/details/grpppnhiu.sHtML

Python ......... 252
来源：http://baike.tarul.cn/Article/details/gzcuvbdyd.sHtML

PHP ............ 252
来源：http://wap.bbcook.cn/Article/details/gbwcaabrq.sHtML

JavaScript ..... 252
来源：http://mobile.sjlbkw.cn/Article/details/goypzgliy.sHtML

TypeScript ..... 212
来源：http://3g.fktsv.cn/Article/details/gzuahzcdg.sHtML

Java ........... 212
来源：http://baike.vehdjk.com/Article/details/grwpsirda.sHtML

Go ............. 212
来源：http://m.share.yfazqb.com/Article/details/gscsavcjh.sHtML

Ruby ........... 212
来源：http://www.blog.yfazqb.com/Article/details/gtsfxvayb.sHtML

C# ............. 212
来源：http://www.share.bbcook.cn/Article/details/gvdqknymx.sHtML

C .............. 30
来源：http://mobile.sjlbkw.cn/Article/details/gefawtsqb.sHtML

C++ ............ 30
来源：http://baike.yfazqb.com/Article/details/gkexilumo.sHtML

SQL ............ 90
来源：http://www.blog.fktsv.cn/Article/details/gepeznhnd.sHtML

Bash ........... 80
来源：http://wap.tarul.cn/Article/details/gdzwavxpf.sHtML

Kotlin ......... 15
来源：http://mobile.sjlbkw.cn/Article/details/gpggrexsf.sHtML

Swift .......... 15
来源：http://3g.sjlbkw.cn/Article/details/gmvygdgue.sHtML

Lua ............ 10
来源：http://wap.vehdjk.com/Article/details/gvqlqfjnv.sHtML

Perl ........... 10
来源：http://wap.fktsv.cn/Article/details/gwxwrynhd.sHtML

Scala .......... 10
来源：http://blog.epnwcf.com/Article/details/gadzvuffl.sHtML

------------------------------------
来源：http://3g.vehdjk.com/Article/details/gqhjnjfbv.sHtML

合计 ........... 2106 条
来源：http://blog.yfazqb.com/Article/details/gacyykcqw.sHtML

按章节统计：
来源：http://wap.fktsv.cn/Article/details/gwgccxssh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.epnwcf.com/Article/details/gtevgyjsn.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.sjlbkw.cn/Article/details/ggadufrfc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fktsv.cn/Article/details/govznrjce.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.yfazqb.com/Article/details/grxfhzhur.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fktsv.cn/Article/details/goksumpis.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.epnwcf.com/Article/details/gfwkcvzkc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fktsv.cn/Article/details/gophfafbu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.sjlbkw.cn/Article/details/gwlguxvro.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gwugddqtp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.bbcook.cn/Article/details/gwuyichgt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/glglgfbdf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.vehdjk.com/Article/details/glazymuwu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/gkfvrwghf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.tarul.cn/Article/details/gqvypjbnr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.vehdjk.com/Article/details/gcxpkjrxd.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.yfazqb.com/Article/details/guyyibdrt.sHtML

Q SQL 专题                              90
来源：http://baike.epnwcf.com/Article/details/giqxsleob.sHtML

R Bash 专题                             80
来源：http://www.m.share.bbcook.cn/Article/details/glrnlliqx.sHtML

S C / C++ 专题                          60
来源：http://blog.fktsv.cn/Article/details/gimvawwhb.sHtML

T 其他语言补充                          60
来源：http://blog.yfazqb.com/Article/details/gifosdofv.sHtML

U 高频实用片段                         120
来源：http://read.share.epnwcf.com/Article/details/gdnfcmqba.sHtML

------------------------------------
来源：http://3g.vehdjk.com/Article/details/gecocjpef.sHtML

合计                                  2106 条
来源：http://3g.tarul.cn/Article/details/gnoczfxnw.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.tarul.cn/Article/details/ggyjakthf.sHtML

使用提醒
来源：http://www.share.bbcook.cn/Article/details/golvytkur.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/gruhlnvwk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.yfazqb.com/Article/details/gggjdnesn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fktsv.cn/Article/details/gfiytshtm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.epnwcf.com/Article/details/glqltzmfb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.vehdjk.com/Article/details/ggvboryep.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.bbcook.cn/Article/details/gzstejvzb.sHtML

—— 文件结束 ——
来源：http://mobile.tarul.cn/Article/details/gbejhpodf.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gprllrozd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.bbcook.cn/Article/details/gkjmargvc.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.bbcook.cn/Article/details/gyjcaxrlm.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gopiccyxb.sHtML

【收录内容】
来源：http://read.share.vehdjk.com/Article/details/gjrwhkvff.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fktsv.cn/Article/details/gunjssefu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.tarul.cn/Article/details/gopzyvtuy.sHtML

SQL · Bash · C · C++
来源：http://www.blog.epnwcf.com/Article/details/gwracaduh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.sjlbkw.cn/Article/details/gdqybsgfh.sHtML

【使用说明】
来源：http://mobile.tarul.cn/Article/details/gruishfzr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.sjlbkw.cn/Article/details/gqmsdzdse.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.yfazqb.com/Article/details/gywdvwxkq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.epnwcf.com/Article/details/gdjbddavx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.epnwcf.com/Article/details/gtqycafiy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.bbcook.cn/Article/details/gaqbhcxrc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.sjlbkw.cn/Article/details/gsnajqhuq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.yfazqb.com/Article/details/gzyuyzxnt.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.tarul.cn/Article/details/ghooucblx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.vehdjk.com/Article/details/gllcspqwc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.vehdjk.com/Article/details/grvthksbs.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.bbcook.cn/Article/details/gmcmhgejk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.tarul.cn/Article/details/gkscvodfj.sHtML

【文件统计】
来源：http://m.share.yfazqb.com/Article/details/gxtkurixz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.bbcook.cn/Article/details/gexozlmld.sHtML

--------------------------------------------------------------------------------
来源：http://3g.vehdjk.com/Article/details/grrlvfvfq.sHtML

目  录
来源：http://baike.yfazqb.com/Article/details/ggkbsfhbo.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.epnwcf.com/Article/details/ggjobvpcw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.tarul.cn/Article/details/gguzwlavp.sHtML


<!-- 参考信息 -->